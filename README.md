# dales_nh3
 The addition of ammonia to DALES
 
 This README file notes the changes made to the code
 
 - _v00_dales-master:
	Original DALES code
	* BUGFIX: modradiation.f90 
		line 253:	use modsurfdata,  only : tauField 
					--> use modsurfdata,  only : tauField, lrsAgs
		line 342: 	tauField(i,j) = tauc 
					--> if (lrAgs) tauField(i,j) = tauc
