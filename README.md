# PS4-Show-Notify
A simple payload to display pop-up notifications.

Just change the notifications that I leave in the examples for the ones you decide before building and enjoy.
```c
#include "ps4.h"

int _main(void) {
  // Init and resolve libraries
  initKernel();
  initLibc();
  jailbreak();

  // Pop-up notifications to show
  printf_notification("PS4 Show Notify by GamerHack");
  
  sceKernelSleep(1); 
  printf_notification("This is an Example");
  
  sceKernelSleep(1); 
  printf_notification("This is another Example");
  
  sceKernelSleep(1); 
  printf_notification("This is all, Bye!");
  return 0;
  }
```

