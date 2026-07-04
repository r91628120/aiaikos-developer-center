# Engine Design Standard

## Engine 責任

Engine 只做資料分析與規則判斷，不處理 UI。

## 基本格式

```js
class WeatherEngine {
  constructor(options = {}) {}
  analyze(input) {
    return { success: true, result: {} };
  }
}
```

## Engine 清單

- WeatherEngine
- WeatherFusionEngine
- CropEngine
- DiseaseEngine
- PestEngine（預留）
- PhysiologyEngine（預留）
- NutritionEngine（預留）
- DecisionEngine
- PromptEngine
- SimulationEngine（預留）
