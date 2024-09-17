# Olah Data Semarang
# WhatsApp : +6285227746673
# IG : @olahdatasemarang_
# Fitting regression analysis of fractional response (responses) models Use frm With (In) R Software
install.packages("remotes")
remotes::install_github("cran/frm")
library("frm")
frm = read.csv("https://raw.githubusercontent.com/timbulwidodostp/frm/main/frm/frm.csv",sep = ";")
# Estimation Fitting regression analysis of fractional response (responses) models Use frm With (In) R Software
y <- frm$y
X <- cbind(frm$X1, frm$X2)
colnames(X) <- c("frm$X1","frm$X2")
rownames(X) <- rownames(X)
# Fractional logit regression model
frm(y,X,linkfrac="logit")
# Binary component of a two-part model - logit specification
frm(y,X,linkbin="logit",type="2Pbin",inf=1)
# Fractional component of a two-part model - probit specification
frm(y,X,linkbin="logit",type="2Pbin",inf=1)
# Fitting regression analysis of fractional response (responses) models Use frm With (In) R Software
# Olah Data Semarang
# WhatsApp : +6285227746673
# IG : @olahdatasemarang_
# Finished