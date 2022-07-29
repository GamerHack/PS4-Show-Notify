# PS4-Show-Notify
A simple payload to display pop-up notifications.

Change the notifications I leave in the examples to the ones you decide before building, it is also possible to delay the timing of a notification by editing the `sceKernelSleep(X)` function; placing a number instead of `(X)` that will delimit the delay in milliseconds as specified.
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

