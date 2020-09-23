<div align="center">

## CMOS Password Clear Utility


</div>

### Description

Purpose:- Save Time and Labour while clearing CMOS setup password..

Now you donn't need to open your computer and make jumper setting for clearing CMOS setup password. Here is the utility for that purpose. 100% tested on IBM or IBM compatible PC.
 
### More Info
 


<span>             |<span>
---                |---
**Submitted On**   |
**By**             |[Nitin Jindal](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByAuthor/nitin-jindal.md)
**Level**          |Advanced
**User Rating**    |5.0 (10 globes from 2 users)
**Compatibility**  |C, C\+\+ \(general\), Borland C\+\+
**Category**       |[Security](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByCategory/security__3-14.md)
**World**          |[C / C\+\+](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByWorld/c-c.md)
**Archive File**   |[](https://github.com/Planet-Source-Code/nitin-jindal-cmos-password-clear-utility__3-6596/archive/master.zip)





### Source Code

```
#include <stdio.h>
#include <dos.h>
#include <conio.h>
int main(void)
{
printf("\n CMOS Clear Utility v1.0");
printf("\n Developed by: Nitin Jindal");
printf("\n Press any key to clear CMOS");
getch();
outportb(0x70,0x2E);
outportb(0x71,0xFF);
printf("\n CMOS cleared..Please restart your pc");
return 0;
}
```

