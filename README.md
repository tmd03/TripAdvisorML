# TripAdvisorML
ML project in Zerobase
Developed a machine learning-based system to recommend personalised travel destinations in Korea based on users' tastes and preferences.
This way, We'll be able to recommend lesser-known destinations in the country.

1. **Improving the user experience** : Increase user satisfaction and reduce travel planning time with personalised recommendations
2. **Business model creation and technology expansion** : Expanding into areas such as customised travel packages and food shopping using recommendation systems

```bash
DS26_presentation.pdf
```

## Raw Data 
https://www.aihub.or.kr/aihubdata/data/view.do?currMenu=&topMenu=&aihubDataSe=data&dataSetSn=71776 (Captital Region)

https://www.aihub.or.kr/aihubdata/data/view.do?currMenu=&topMenu=&aihubDataSe=data&dataSetSn=71778 (Eastern Region)

https://www.aihub.or.kr/aihubdata/data/view.do?currMenu=&topMenu=&aihubDataSe=data&dataSetSn=71779 (Western Region)

https://www.aihub.or.kr/aihubdata/data/view.do?currMenu=&topMenu=&aihubDataSe=data&dataSetSn=71780 (Jeju and Islands)

## Used Data
**- TN_TRAVELLER_MASTER : Traveller's basic information**
  - Traveller ID, Gender, Age Group, Preferred City, Preferred City District, Travel Style, Residence, Destination

**- TN_TRAVEL : Basic travel information**
  - Traveller ID, Travel ID, Travel Purpose, Travel Date
    
**- TN_VISIT_AREA_INFO : Visit Area Information**
  - Trip ID, Name of visit area, Date of visit, Address, Coordinates, Type of visit area
</br>
- TC_SGG: City and district code
</br>
- TC_CODEA, TC_CODEB : Code list table

## Processing
Input : Gender, Age, Travel Style, Residence

-> Output : Recommended City, Top 10 recommended destinations in City

## EDA
```bash
EDA_1.ipynb
```
> Conducted EDA of raw data to select effective input data

## MODEL
- Catboost(weight) **(adopted)**
  ```bash
  catboost_weight.ipynb
  ```
- LightGBM
  ```bash
  ML_lgbm_final.ipynb
  ```
- Content-based Filtering


