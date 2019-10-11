# DM_HW
##資料探勘191012R作業

##變異數函數
a = function(data){
  result = 0
  for (i in 1:length(data)){
    result = ((result - mean(data))**2)/(length(data)-1)
  }
  return(result)
}
a(1:10)


##99乘法表矩陣
m = matrix(nrow = 9,ncol =  9)
for (i in 1:9){
  for (j in 1:9){
    m[i, j] = i*j
  }
}
