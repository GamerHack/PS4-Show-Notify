# PS4-Show-Notifi
A simple payload to display pop-up notifications.

You should only change the notifications that I leave by default for the ones you decide, you can also delay the time to show a notification in "sceKernelSleep(X);" placing a number instead of (X).
```c
#include "ps4.h"

int _main(void) {
  // Init and resolve libraries
  initKernel();
  initLibc();

  // Pop-up notifications to show
  printf_notification("PS4 Show Notifi by GamerHack");
  
  sceKernelSleep(1); 
  printf_notification("This is an Example");
  
  sceKernelSleep(1); 
  printf_notification("This is another Example");
  
  sceKernelSleep(1); 
  printf_notification("This is all, Bye!");
  return 0;
  }
```

