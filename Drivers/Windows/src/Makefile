all:	../ATLAS_DRV.exe ../ATLAS_D64.exe

../ATLAS_DRV.exe:	ATLAS_DRV.7z
	cat 7zSD.sfx config.txt ATLAS_DRV.7z > ../ATLAS_DRV.exe

../ATLAS_D64.exe:	ATLAS_D64.7z
	cat 7zSD.sfx config.txt ATLAS_D64.7z > ../ATLAS_D64.exe

ATLAS_DRV.7z:
	cd files && 7za a ../$@ *
	cd dpinst && 7za a ../$@ dpinst.exe

ATLAS_D64.7z:
	cd files && 7za a ../$@ *
	cd dpinst64 && 7za a ../$@ dpinst.exe

clean:
	rm ATLAS_DRV.7z ATLAS_D64.7z
