# Thoracic Infection 3-Month Survival Predictor

A web-based clinical prediction tool for estimating 3-month survival probability in patients with thoracic infection, based on Cox proportional hazards regression model.

## 🔬 Model Information

- **Sample Size**: 1,115 patients from multicenter cohort
- **Events**: 153 deaths within 3 months
- **C-index**: 0.841

### Predictors

| Variable | Coefficient (β) | HR (95% CI) | P Value |
|----------|-----------------|-------------|---------|
| Age (per year) | 0.0589 | 1.06 (1.05–1.07) | <0.001 |
| Urea (per mmol/L) | 0.0406 | 1.04 (1.03–1.05) | <0.001 |
| Albumin (per g/L) | -0.0494 | 0.95 (0.93–0.97) | <0.001 |
| Hospital-acquired infection | 0.6712 | 1.96 (1.37–2.80) | <0.001 |

### Prediction Formula

```
Linear Predictor (LP) = 0.0589×Age + 0.0406×Urea − 0.0494×Albumin + 0.6712×Hospital

3-Month Survival Probability = 0.9274^exp(LP)
```

## 🚀 Live Demo

Visit: `https://YOUR-USERNAME.github.io/YOUR-REPO-NAME`

## 📱 Features

- Responsive design (mobile-friendly)
- Real-time calculation
- Visual risk stratification
- No server required (pure HTML/CSS/JS)

## ⚠️ Disclaimer

This tool is intended for **research and educational purposes only**. Clinical decisions should be made by qualified healthcare professionals considering all relevant patient factors.

## 📄 License

MIT License
