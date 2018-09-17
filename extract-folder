function extract-folder () {
for i in `ls -1`
	do
		cd $i
		pwd
		
		unset g_result
		files=`ls -1`
		echo $files | grep -q '1.rar' 
		
		g_result=$?
		echo $g_result
		
	
		if [[ $g_result == 1 ]] 
			then
				echo "extract *.rar"
				unrar -y x *.rar 
	
		elif [[ $g_result == 0 ]] 
				then
				echo "extract 1.rar"
				unrar -y x *1.rar
		else
				echo "Not Sure"
		fi
		 

		cd ..
		pwd
		sleep 0.5
	done

}
