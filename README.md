# A modified version of the [BGLR R-package](https://github.com/gdlc/BGLR-R) that can use [bigmmemory](https://cran.r-project.org/web/packages/bigmemory/index.html) objects as inputs.

**Developer**: Paulino Perez-Rodriguez (perpdgo@gmail.com)

NOTE: The user interface is identical to that of BGLR. The example below illustrates the use of `bigBGLR` further examples are provided @ [BGLR-examples](https://github.com/gdlc/BGLR-R/blob/master/README.md).


```R
library(bigBGLR)
data(wheat)
X=as.big.matrix(wheat.X)
ETA=list(list(X=X,model="BRR"))
fm=BGLR(y=wheat.Y[,1],ETA=ETA)

```
