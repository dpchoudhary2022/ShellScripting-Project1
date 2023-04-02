// create a digital clock by shell script

$ date 
$ date +%T
$ date +%T; sleep 1s;
$ date +%T; sleep 1s; date +%T; sleep 1s; date +%T; sleep 1s;
$ clear; date date +%T; sleep 1s; date +%T; sleep 1s;
$ vi digital_watch.sh

--------------------------------------------------------------------
         #!/bin/bash
         while true 
         do
               clear
               echo $(date +%T)
               sleep 1s
        done 

        save & exit vi editior now
----------------------------------------------------------------------
$ chmod 777 digital_watch.sh
$ vi digital_watch.sh
--------------------------------------------------------------------
         #!/bin/bash
         Red=$'\e[1;31m'
         Blue=$'\e[1;34m'
         Green=$'\e[1;32

         while true 
         do
               clear
               echo $Red $(date +%T)
               sleep 1s
        done 

        save & exit vi editior now
----------------------------------------------------------------------
$ ./digital_watch.sh
