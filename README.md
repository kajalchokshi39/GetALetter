# GetALetter

#Replicate 4.978 seconds
#system.time(replicate(1000000, alphabet()))

#Lapply 6.9974
#start <- Sys.time()
#results <- unlist(lapply(1:1000000,alphabet))
#end <- Sys.time()
#end - start

#Parallel Processing Mclapply 7.725
#start <- Sys.time()
#results <- unlist(mclapply(1:1000000,alphabet,mc.cores = 4))
#end <- Sys.time()
#end - start

#ParLapply
#library(parallel)
#detectCores()
# Calculate the number of cores
#no_cores <- detectCores() - 1

# Initiate cluster 2.219383955
#cl <- makeCluster(no_cores)

#start <- Sys.time()
#parLapply(cl, 1:1000000, alphabet)
#end <- Sys.time()
#end-start

#stopCluster(cl)
