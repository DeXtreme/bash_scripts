#! /bin/sh
# This script lists the contents of the usr/local
# directory or the given directory path


list_contents(){
	for file_name in $1/*; do  # Loop through contents of the directory
		echo "${file_name}"
	done
}

if [ $# -eq 1 ]; then  # Check if an argument was given
	if [ -d $1 ]; then  #Check if argument is valid path
		echo "Listing files and folders in \e[1;34m$1\e[m"
		list_contents $1
	else
		echo "Invalid path"
		echo "Usage : listdir.sh [path/to/directory]"
	fi
elif [ $# -eq 0 ]; then # Check if no arguemnt was given
	echo "Listing files and folders in \e[1;34m/usr/local\e[m"
	list_contents /usr/local
else
	echo "Usage : listdir.sh [path/to/directory]"
fi
