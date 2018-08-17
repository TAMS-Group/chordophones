# chordophones
ROS/Gazebo models of fretted stringed instruments.

##chordophones

ROS/Gazebo object models of a few fretted stringed music instruments:
(electric) bass, guitar, ukule, pipa.
We plan to use these models as affordance-rich demo objects for grasp and manipulation planning and learning, 
both in simulation and on our real robots.

To make all of this sound more impressive (pun intended), we simply had to use the
scientific classificiation term for the package name.
Actually, there is no sound yet, but we are planning a Gazebo plugin
that observes string motion and generates MIDI/audio output.

##Getting Started

Well, these are complicated objects. You probably want to use them together with humanoid robots and multifingered hands.

For example, using our modified PR2 robot with Shadow Dexterous Hand:

roscore
roslaunch tams_pr2_moveit_config demo.launch
roslaunch chordophones spawn_paula.launch
roslaunch chordophones concierto_de_aranjuez.launch 

Just kidding, we're not there yet. Try this instead:

roslaunch chordophones tams_pr2_paula_chromatic_scale.launch

##Known Issues
