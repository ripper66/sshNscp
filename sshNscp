#!/bin/bash
#
# A simple bash script that do SSH and SCP STDIN from a text file.
#
echo "Executing SSH & SCP..."
cat << "EOF"
echo "========================================="
              __       ___
   __________/ /_     ( _ )      ______________
  / ___/ ___/ __ \   / __ \/|   / ___/ ___/ __ \
 (__  |__  ) / / /  / /_/  <   (__  ) /__/ /_/ /
/____/____/_/ /_/   \____/\/  /____/\___/ .___/
                                       /_/
EOF
echo "========================================="
echo " "
for server in $(cat IP.txt) # <-- Please modified this
do
ssh-copy-id root@"$server" && scp file.txt root@"$server":/tmp/ # <-- and change the filename for SCP
done
wait
