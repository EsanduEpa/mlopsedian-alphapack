# mlopsedian-alphapack

Initial dataset had 47 columns
45 of them were features (excluding target variable = flood_risk_score, record_id)
Initially my intention was to do a linear regression, therefore i removed skewed data and used provided qmap,yejohnson,log1p where ever possible
So the features count came down to 23

'landcover','soil_type','water_supply','electricity','road_quality','water_presence_flag','historical_flood_count','infrastructure_score','distance_to_river_m_log1p','population_density_per_km2_log1p','rainfall_7d_mm_log1p','monthly_rainfall_mm_log1p','nearest_hospital_km_log1p','nearest_evac_km_log1p','elevation_m_yeojohnson','drainage_index_yeojohnson','ndvi_qmap','ndwi_qmap','built_up_percent_qmap','seasonal_index','terrain_roughness_index','socioeconomic_status_index','extreme_weather_index'

Then I extracted categorical variables (6 were)
replaced their NaNs with "Unknown" and then did one-hot encoding
<img width="174" height="98" alt="image" src="https://github.com/user-attachments/assets/b120d47c-f3b1-4fcf-82f1-ce0f021bc61a" />
Then those 5 columns became -> 26 [automatically original columns dissapear]

So now i had 49 total features

I also replaced 17 numberical column's NaN values with their means

#Then the first submission was made

Then I exploded features
I called a function to make (17*16)/2 = 136 
136 * 4(+-/*) = 544 features newly
#Then I made the second submission

Then I took only the best 50 features and ran the model on that 50 features only
#Then I did the third submission

