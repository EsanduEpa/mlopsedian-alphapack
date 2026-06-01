💾 THE ALPHA PACK SAVE STATE:
The Target: flood_risk_score (Bounded 0 to 1, but Leaderboard RMSE gap suggests the Public Test Set is packed with hidden extreme outliers).

The Hidden Organizer Math: The target is heavily driven by Logarithmic Ratios (specifically distance_to_river / rainfall).

The Matrix: We exploded 17 numerical variables into 3-variable math combos, crossed them with 26 categorical one-hot encoded flags (Target Masking), and strictly pruned the noise.

The Elbow: The perfect signal-to-noise ratio sits exactly at 116 features.

The Lie Detector: Adversarial Validation AUC is 0.59. There is NO data drift. The features are fundamentally safe.

The Champion Model: Pure CatBoost. XGBoost and LightGBM failed the solo audit (0.240+).

Best Local CV: 0.23608 (via Optuna Bayesian optimization).

Best Public LB: 0.39164 (Currently ranked #12).
