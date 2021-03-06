# List of Models

### Benchmark Models

- `simplegeometricmean.py` (Geometric Mean of [Store, DayOfWeek, Promo] Groups)
    - Private Score: 0.15996, Public Score: 0.15390
    - Features: Store, DayOfWeek, Promo
- `simplemedian.py` (Median of [Store, DayOfWeek, Promo] Groups)
    - Private Score: 0.14598, Public Score: 0.14001
    - Features: Store, DayOfWeek, Promo

### scikit-learn Models

- `linearregression-independent.py` (Independent Regression Models)
    - Private Score: 0.16939, Public Score: 0.14867
    - Features: Promo, SchoolHoliday, DayOfWeek (one-hot encoded), StateHoliday (one-hot encoded)
- `linearregression-independent2.py` (Independent Regression Models)
    - Private Score: 0.16405, Public Score: 0.14499
    - Features: Promo, DayOfWeek (one-hot encoded)
- `linearregression-independent3.py` (Independent Regression Models)
    - Private Score: 0.16411, Public Score: 0.14511
    - Features: Promo, DayOfWeek (one-hot encoded), StateHoliday (one-hot encoded)
- `linearregression-independent4.py` (Independent Regression Models)
    - Private Score: 0.16209, Public Score: 0.14587
    - Features: Promo, SchoolHoliday, Year, Month, DayOfWeek (one-hot encoded), StateHoliday (one-hot encoded), AvgCustStore, AvgCustStoreMonth
- `linearregression-independent-log.py` (Independent Regression Models)
    - Private Score: 0.15522, Public Score: 0.13742
    - Features: Promo, SchoolHoliday, Year, Month, DayOfWeek (one-hot encoded), StateHoliday (one-hot encoded), AvgCustStore, AvgCustStoreMonth
- `linearregression-single.py` (Single Regression Model)
    - Private Score: 0.42820, Public Score: 0.42460
    - Features: Store, Promo, SchoolHoliday, DayOfWeek (one-hot encoded), StateHoliday (one-hot encoded), CompetitionDistance, StoreType (one-hot encoded), Assortment (one-hot encoded)
- `linearregression-single2.py` (Single Regression Model)
    - Private Score: 0.26838, Public Score: 0.26738
    - Features: Store, Promo, SchoolHoliday, Year, Month, DayOfWeek (one-hot encoded), StateHoliday (one-hot encoded), CompetitionDistance, StoreType (one-hot encoded), Assortment (one-hot encoded), AvgCustStore, AvgCustStoreMonth, AvgCustStoreYear
- `randomforestregression-independent-log.py` (Independent RF Regression Models)
    - Private Score: 0.14536, Public Score: 0.13748
    - Features: Promo, SchoolHoliday, Year, Month, DayOfWeek (one-hot encoded), StateHoliday (one-hot encoded), AvgCustStore, AvgCustStoreMonth
- `randomforestregression-single2.py` (Single RF Regression Model)
    - Private Score: 0.14726, Public Score: 0.14016
    - Features: Store, Promo, SchoolHoliday, Year, Month, DayOfWeek (one-hot encoded), StateHoliday (one-hot encoded), CompetitionDistance, StoreType (one-hot encoded), Assortment (one-hot encoded), AvgCustStore, AvgCustStoreMonth, AvgCustStoreYear
- `ridgeregression.py` (Independent Ridge Regression Models)
    - Private Score: 0.16179, Public Score: 0.14526
    - Features: Promo, SchoolHoliday, Year, Month, DayOfWeek (one-hot encoded), StateHoliday (one-hot encoded), AvgCustStore, AvgCustStoreMonth

### XGBoost Models

- `xgboostregressor.py`
    - Private Score: 0.16360, Public Score: 0.14958
    - Features: Promo, SchoolHoliday, DayOfWeek, StateHoliday
- `xgboostregressor2.py`
    - Private Score: 0.13205, Public Score: 0.11356
    - Features: Store, DayOfWeek, Year, Month, DayOfMonth, Open, Promo, StateHoliday, SchoolHoliday, StoreType, Assortment, CompetitionDistance, Promo2
- `xgboostregressor-log.py`
    - Private Score: 0.12728, Public Score: 0.10754
    - Features: Store, DayOfWeek, Year, Month, DayOfMonth, Open, Promo, StateHoliday, SchoolHoliday, StoreType, Assortment, CompetitionDistance, Promo2
- `xgboostregressor-log2.py`
    - Private Score: 0.13264, Public Score: 0.11770
    - Features: Store, Year, Month, YearMonth, Open, Promo, SchoolHoliday, CompetitionDistance, Promo2, CompetitionOpenSinceYear, StateHoliday, DayOfWeek, StateHolidayBinary, StoreType, Assortment
- `xgboostregressor-log3.py`
    - Private Score: 0.12511, Public Score: 0.11315
    - Features: Store, DayOfWeek, Year, Month, DayOfMonth, Open, Promo, StateHoliday, SchoolHoliday, StoreType, Assortment, CompetitionDistance, Promo2, AvgCustStore, AvgCustStoreMonth
- `xgboostregressor-log4.py`
    - Private Score: 0.12708, Public Score: 0.11219
    - Features: Store, DayOfWeek, Year, Month, DayOfMonth, Open, Promo, SchoolHoliday, CompetitionDistance, Promo2, WeekOfYear, CompetitionOpenInterval, PromoOpenInterval, IsPromoMonth, StoreType, Assortment, StateHoliday
- `xgboostregressor-log5.py`
    - Private Score: 0.12305, Public Score: 0.11276
    - Features: Store, DayOfMonth, Week, Month, Year, DayOfYear, DayOfWeek, Open, Promo, SchoolHoliday, StateHoliday, StoreType, Assortment, CompetitionDistance, CompetitionOpenYearMonthInteger, AvgSales, AvgCustomers, AvgSalesPerCustomer
- `xgboostensemble.py`
    - Private Score: 0.11880, Public Score: 0.10640
    - Models: Predictions from xgboostregressor-log5 & xgboostregressor-log
