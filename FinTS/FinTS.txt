# Olah Data Semarang
# WhatsApp : +6285227746673
# IG : @olahdatasemarang_
# Box-Pierce and Ljung-Box autocorrelation test Use AutocorTest And Box.test (FinTS) With (In) R Software
install.packages("FinTS")
library("FinTS")
library("stats")
FinTS = read.csv("https://raw.githubusercontent.com/timbulwidodostp/FinTS/main/FinTS/FinTS.csv",sep = ";")
# Estimation Box-Pierce and Ljung-Box autocorrelation test Use AutocorTest And Box.test (FinTS) With (In) R Software
x <- FinTS
Box_Ljung_test_1 <- AutocorTest(FinTS, 5)
Box_Ljung_test_1
Box_Ljung_test_2 <- AutocorTest(FinTS, 5, df=4)
Box_Ljung_test_2
Box_Ljung_test_3 <- Box.test (x, lag = 1, type = "Ljung")
Box_Ljung_test_3
Pierce_test <- Box.test (x, lag = 1)
Pierce_test
# Box-Pierce and Ljung-Box autocorrelation test Use AutocorTest And Box.test (FinTS) With (In) R Software
# Olah Data Semarang
# WhatsApp : +6285227746673
# IG : @olahdatasemarang_
# Finished