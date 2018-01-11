A straightforward and easy to use timer and various time, timing and timer features. 

simplifies the overly verbose std::chrono from -std=c++11

Basic use
mlib::Timer timer;
timer.tic();
// do stuff
timer.toc();
cout<<timer<<endl;


or 

mlib::Timer iteration;
for(int i=0;i<1000;++i){
iteration.tic();
// do stuff
iteration.toc();
}
cout<<iteration<<endl;
for a nice table with total, min, max,median etc in human readable format

or output several timers in a nice table: 

mlib::Timer a,b,c,d;
// time some stuff:

cout<<{a,b,c,d}<<endl;

contains basic functions such as 
sleep with high precision


