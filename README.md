To use OpenCV, the source must be compiled, which takes about 2 hours on my PC. So I store binaries here to avoid compiling. The binaries are for Windows 10, other operting systems are not tested and will probably not work.

To use:
- put bin direction into path to be found by windows
- to include the directories include and lib (.rar unpacked) in Eclipse:
- properties - C/C++ Build - Settings - GCC C++ Compiler - Includes - -l c:\....\include
- properties - C/C++ Build - Settings - MinGW C++ Linker - Libraries - -L c:\...\lib
- properties - C/C++ Build - Settings - MinGW C++ Linker - Libraries - -l opencv_core454.dll (all .a files withouth extension)

usage in code:
#include <opencv2/core.hpp>
#include <opencv2/highgui.hpp>
cv::Mat image = cv::imread("...");
