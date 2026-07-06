# Olah Data Semarang
# WhatsApp : +6285227746673
# IG : @olahdatasemarang_
# Compute Royston's D for a Cox model Use royston (survival) With (In) R Software
install.packages("survival")
library("survival")
# Estimation Compute Royston's D for a Cox model Use royston (survival) With (In) R Software
royston = read.csv("https://raw.githubusercontent.com/timbulwidodostp/royston/main/royston/royston.csv",sep = ";")
royston_1 <- coxph(Surv(time, status == 2) ~ age + log(bili) + edema + albumin + stage + copper, data = royston)
royston_2 <- coxph(Surv(time, status == 2) ~ age + log(bili) + edema + albumin + stage, data = royston)
royston_3 <- coxph(Surv(time, status == 2) ~ age + log(bili) + edema + albumin, data = royston)
royston_4 <- coxph(Surv(time, status == 2) ~ age + log(bili) + edema, data = royston)
royston_5 <- coxph(Surv(time, status == 2) ~ age + log(bili) + edema, data = royston)
royston_6 <- coxph(Surv(time, status == 2) ~ age + log(bili), data = royston)
royston_7 <- coxph(Surv(time, status == 2) ~ age, data = royston)
royston_1 <- royston(royston_1)
royston_2 <- royston(royston_2)
royston_3 <- royston(royston_3)
royston_4 <- royston(royston_4)
royston_5 <- royston(royston_5)
royston_6 <- royston(royston_6)
royston_7 <- royston(royston_7)
royston_1
royston_2
royston_3
royston_4
royston_5
royston_6
royston_7
# Compute Royston's D for a Cox model Use royston (survival) With (In) R Software
# Olah Data Semarang
# WhatsApp : +6285227746673
# IG : @olahdatasemarang_
# Finished