# Kaggle-IEEE-CIS-Fraud-Detection-Project-C-

Kaggle-IEEE-CIS-Fraud-Detection項目的要旨是應用真實生活中來自Vesta公司(電子支付公司)交易數據以及機器學習，提高盜刷偵測之準確率，加強顧客服務品質。

這個比賽中所使用的數據十分龐大，為1.25GB(一百萬筆交易數據)。因為數據規模不小，所以使用Google Colab Pro GPU 處理，否則十分耗時且電腦無法消化。

數據來源: Vesta Corporation 與 IEEE-CIS 於 2019年7月在Kaggle舉辦的 Fraud Detection(盜刷偵測)比賽:https://www.kaggle.com/c/ieee-fraud-detection/overview

分數評判: 根據ROC curve between the predicted probability and the observed target。

所應用之方法:

1. 通過EDA觀察數據，填補缺失值。
2. 應用Random OverSampling(Up-Scaling)處理Training Dataset標籤分布不均之問題(Ture: 3.499%, False: 96.5%)(相較Downsampling, SMOTE, Random OverSampling根據所需時間、準確率，表現最好)
3. 數種 Encoding, Feature Engineering方法。
4. 以XgBoost在調參後所達到之最高分數: 0.910459。



