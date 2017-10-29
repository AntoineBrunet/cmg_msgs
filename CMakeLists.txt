cmake_minimum_required(VERSION 2.8.3)
project(cmg_msgs)

find_package(catkin REQUIRED genmsg std_msgs)

add_message_files(FILES
		  State.msg
		  Signal.msg
		  Speed.msg
		  SpeedList.msg
		  GimbalTarget.msg
                  Commande.msg
                  Commande_moteur.msg
                 )

generate_messages(DEPENDENCIES std_msgs)

catkin_package(DEPENDS std_msgs)

