# AIAKOS System Overview

AIAKOS（AI Agriculture Knowledge Operating System）是 AI農業教育平台的共用核心，負責提供氣象、作物、病害、蟲害、決策、模擬、提示詞與資料管理能力。

## 核心原則

- 所有平台共用同一套 Engine、Service、JSON Data。
- 不在各平台重複開發同功能。
- Engine 不操作 DOM；UI 僅負責呈現。
- JSON 欄位需版本化、可追蹤來源、可向下相容。

## 平台接入

- AI農業氣象教練：WeatherEngine + WeatherFusionEngine + DecisionEngine
- AI植物診療師：WeatherEngine + DiseaseEngine + PromptEngine
- AI智慧農業決策中心：WeatherEngine + CropEngine + DecisionEngine
- AI農業經營大富翁：CropEngine + MarketEngine + SimulationEngine
- AI智慧養殖：IoT Engine + AquacultureEngine + AlertEngine
- AI花藝設計師學院：FloralDesignEngine + EvaluationEngine + PromptEngine
