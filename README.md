# Doomsday
computes day of the week for any date between Jan. 1, 2000 and Dec. 31, 2099


import javax.swing.JOptionPane;
String yr;
yr = JOptionPane.showInputDialog ("choose a year between 2000 and 2099");
int y = Integer.parseInt(yr);
String mn;
mn = JOptionPane.showInputDialog ("choose a month between January(1) and December (12)");
int m = Integer.parseInt(mn);
String dy;
dy = JOptionPane.showInputDialog ("choose a date (between 1 - 31 for January, March, May, July, August, October, December, between 1 - 30 for April, June, September, November, between 1-28 for February(29 if leap year))");
int d = Integer.parseInt(dy);


int yrr = y - 2000;
int tw = yrr/12;
int re = yrr%12;
int fo = re/4;
int doom = (fo+tw+re+2)%7;
int day;
String date;
int duum;
int d8;
boolean leap = false;

if(y%4 == 0){
  leap = true;
}



Even months except feb
if (m%2 == 0 && m >2) {
  duum = m;
  if (d == duum) {
    day = doom;
    if (day == 0 || day == 7) {
      date = "Sunday";
      println(date);
    } else if (day == 1) {
      date = "Monday";
      println(date);
    } else if (day == 2) {
      date = "Tuesday";
      println(date);
    } else if (day == 3) {
      date = "Wednesday";
      println(date);
    } else if (day == 4) {
      date = "Thursday";
      println(date);
    } else if (day == 5) {
      date = "Friday";
      println(date);
    } else if (day == 6) {
      date = "Saturday";
      println(date);
    }
  } else if (d>duum) {
    d8 = (d-duum)%7;
    day = (d8 + doom)%7;

    if (day == 0 || day == 7) {
      date = "Sunday";
      println(date);
    } else if (day == 1) {
      date = "Monday";
      println(date);
    } else if (day == 2) {
      date = "Tuesday";
      println(date);
    } else if (day == 3) {
      date = "Wednesday";
      println(date);
    } else if (day == 4) {
      date = "Thursday";
      println(date);
    } else if (day == 5) {
      date = "Friday";
      println(date);
    } else if (day == 6) {
      date = "Saturday";
      println(date);
    }
  } else if (d<duum) {
    d8 = (duum-d)%7;
     if(d8 <= doom){
    day = (doom - d8)% 7;
  
  
     if (day == 0 || day == 7) {
    date = "Sunday";
    println(date);
  } else if (day == 1) {
    date = "Monday";
    println(date);
  } else if (day == 2) {
    date = "Tuesday";
    println(date);
  } else if (day == 3) {
    date = "Wednesday";
    println(date);
  } else if (day == 4) {
    date = "Thursday";
    println(date);
  } else if (day == 5) {
    date = "Friday";
    println(date);
  } else if (day == 6) {
    date = "Saturday";
    println(date);
  }
  }
  if(d8>doom){
    day = (doom - d8) + 7;
    if (day == 0 || day == 7) {
    date = "Sunday";
    println(date);
  } else if (day == 1) {
    date = "Monday";
    println(date);
  } else if (day == 2) {
    date = "Tuesday";
    println(date);
  } else if (day == 3) {
    date = "Wednesday";
    println(date);
  } else if (day == 4) {
    date = "Thursday";
    println(date);
  } else if (day == 5) {
    date = "Friday";
    println(date);
  } else if (day == 6) {
    date = "Saturday";
    println(date);
  }
  }
}
}


jan
if (m==1 && leap == false) {
  duum = 3;
if (d == duum) {
    day = doom;
    if (day == 0 || day == 7) {
      date = "Sunday";
      println(date);
    } else if (day == 1) {
      date = "Monday";
      println(date);
    } else if (day == 2) {
      date = "Tuesday";
      println(date);
    } else if (day == 3) {
      date = "Wednesday";
      println(date);
    } else if (day == 4) {
      date = "Thursday";
      println(date);
    } else if (day == 5) {
      date = "Friday";
      println(date);
    } else if (day == 6) {
      date = "Saturday";
      println(date);
    }
  } else if (d>duum) {
    d8 = (d-duum)%7;
    day = (doom + d8)%7;
    if (day == 0 || day == 7) {
      date = "Sunday";
      println(date);
    } else if (day == 1) {
      date = "Monday";
      println(date);
    } else if (day == 2) {
      date = "Tuesday";
      println(date);
    } else if (day == 3) {
      date = "Wednesday";
      println(date);
    } else if (day == 4) {
      date = "Thursday";
      println(date);
    } else if (day == 5) {
      date = "Friday";
      println(date);
    } else if (day == 6) {
      date = "Saturday";
      println(date);
    }
  } else if (d<duum) {
    d8 = (duum-d)%7;
    day = doom - d8;


    if (day == 0 || day == 7) {
      date = "Sunday";
      println(date);
    } else if (day == 1) {
      date = "Monday";
      println(date);
    } else if (day == 2) {
      date = "Tuesday";
      println(date);
    } else if (day == 3) {
      date = "Wednesday";
      println(date);
    } else if (day == 4) {
      date = "Thursday";
      println(date);
    } else if (day == 5) {
      date = "Friday";
      println(date);
    } else if (day == 6) {
      date = "Saturday";
      println(date);
    }
  }
}

if (m==1 && leap == true) {
  duum = 4;
  if (d == duum) {
    day = doom;
    if (day == 0 || day == 7) {
      date = "Sunday";
      println(date);
    } else if (day == 1) {
      date = "Monday";
      println(date);
    } else if (day == 2) {
      date = "Tuesday";
      println(date);
    } else if (day == 3) {
      date = "Wednesday";
      println(date);
    } else if (day == 4) {
      date = "Thursday";
      println(date);
    } else if (day == 5) {
      date = "Friday";
      println(date);
    } else if (day == 6) {
      date = "Saturday";
      println(date);
    }
  } else if (d>duum) {
    d8 = (d-duum)%7;
    day = (doom + d8)%7;
    if (day == 0 || day == 7) {
      date = "Sunday";
      println(date);
    } else if (day == 1) {
      date = "Monday";
      println(date);
    } else if (day == 2) {
      date = "Tuesday";
      println(date);
    } else if (day == 3) {
      date = "Wednesday";
      println(date);
    } else if (day == 4) {
      date = "Thursday";
      println(date);
    } else if (day == 5) {
      date = "Friday";
      println(date);
    } else if (day == 6) {
      date = "Saturday";
      println(date);
    }
  }
   else if (d<duum ) {
    d8 = (duum-d)%7;
    day = doom - d8 + 7;


    if (day == 0 || day == 7) {
      date = "Sunday";
      println(date);
    } else if (day == 1) {
      date = "Monday";
      println(date);
    } else if (day == 2) {
      date = "Tuesday";
      println(date);
    } else if (day == 3) {
      date = "Wednesday";
      println(date);
    } else if (day == 4) {
      date = "Thursday";
      println(date);
    } else if (day == 5) {
      date = "Friday";
      println(date);
    } else if (day == 6) {
      date = "Saturday";
      println(date);
    }
  }
 }



feb
if (m==2 && leap == false) {
    duum = 28;
if(d == duum){
    day = doom;
     if (day == 0) {
    date = "Sunday";
    println(date);
  } else if (day == 1) {
    date = "Monday";
    println(date);
  } else if (day == 2) {
    date = "Tuesday";
    println(date);
  } else if (day == 3) {
    date = "Wednesday";
    println(date);
  } else if (day == 4) {
    date = "Thursday";
    println(date);
  } else if (day == 5) {
    date = "Friday";
    println(date);
  } else if (day == 6) {
    date = "Saturday";
    println(date);
  }
}

 

  else if(d<duum){
  d8 = (duum-d)%7;
  if(d8 <= doom){
    day = (doom - d8)% 7;
  
  
     if (day == 0 || day == 7) {
    date = "Sunday";
    println(date);
  } else if (day == 1) {
    date = "Monday";
    println(date);
  } else if (day == 2) {
    date = "Tuesday";
    println(date);
  } else if (day == 3) {
    date = "Wednesday";
    println(date);
  } else if (day == 4) {
    date = "Thursday";
    println(date);
  } else if (day == 5) {
    date = "Friday";
    println(date);
  } else if (day == 6) {
    date = "Saturday";
    println(date);
  }
  }
  if(d8>doom){
    day = (doom - d8) + 7;
    if (day == 0 || day == 7) {
    date = "Sunday";
    println(date);
  } else if (day == 1) {
    date = "Monday";
    println(date);
  } else if (day == 2) {
    date = "Tuesday";
    println(date);
  } else if (day == 3) {
    date = "Wednesday";
    println(date);
  } else if (day == 4) {
    date = "Thursday";
    println(date);
  } else if (day == 5) {
    date = "Friday";
    println(date);
  } else if (day == 6) {
    date = "Saturday";
    println(date);
  }
  }
}
}
if (m==2 && leap == true) {
    duum = 29;
if(d == duum){
    day = doom;
     if (day == 0) {
    date = "Sunday";
    println(date);
  } else if (day == 1) {
    date = "Monday";
    println(date);
  } else if (day == 2) {
    date = "Tuesday";
    println(date);
  } else if (day == 3) {
    date = "Wednesday";
    println(date);
  } else if (day == 4) {
    date = "Thursday";
    println(date);
  } else if (day == 5) {
    date = "Friday";
    println(date);
  } else if (day == 6) {
    date = "Saturday";
    println(date);
  }
}

 

  else if(d<duum){
  d8 = (duum-d)%7;
  if(d8 <= doom){
    day = (doom - d8)% 7;
  
  
     if (day == 0 || day == 7) {
    date = "Sunday";
    println(date);
  } else if (day == 1) {
    date = "Monday";
    println(date);
  } else if (day == 2) {
    date = "Tuesday";
    println(date);
  } else if (day == 3) {
    date = "Wednesday";
    println(date);
  } else if (day == 4) {
    date = "Thursday";
    println(date);
  } else if (day == 5) {
    date = "Friday";
    println(date);
  } else if (day == 6) {
    date = "Saturday";
    println(date);
  }
  }
  if(d8>doom){
    day = (doom - d8) + 7;
    if (day == 0 || day == 7) {
    date = "Sunday";
    println(date);
  } else if (day == 1) {
    date = "Monday";
    println(date);
  } else if (day == 2) {
    date = "Tuesday";
    println(date);
  } else if (day == 3) {
    date = "Wednesday";
    println(date);
  } else if (day == 4) {
    date = "Thursday";
    println(date);
  } else if (day == 5) {
    date = "Friday";
    println(date);
  } else if (day == 6) {
    date = "Saturday";
    println(date);
  }
  }
}
}


march
if (m==3) {
  duum = 14;
  if (d == duum) {
    day = doom;
    if (day == 0 || day == 7) {
      date = "Sunday";
      println(date);
    } else if (day == 1) {
      date = "Monday";
      println(date);
    } else if (day == 2) {
      date = "Tuesday";
      println(date);
    } else if (day == 3) {
      date = "Wednesday";
      println(date);
    } else if (day == 4) {
      date = "Thursday";
      println(date);
    } else if (day == 5) {
      date = "Friday";
      println(date);
    } else if (day == 6) {
      date = "Saturday";
      println(date);
    }
  } else if (d>duum) {
    d8 = (d-duum)%7;
    day = (d8 + doom)%7;

    if (day == 0 || day == 7) {
      date = "Sunday";
      println(date);
    } else if (day == 1) {
      date = "Monday";
      println(date);
    } else if (day == 2) {
      date = "Tuesday";
      println(date);
    } else if (day == 3) {
      date = "Wednesday";
      println(date);
    } else if (day == 4) {
      date = "Thursday";
      println(date);
    } else if (day == 5) {
      date = "Friday";
      println(date);
    } else if (day == 6) {
      date = "Saturday";
      println(date);
    }
  } else if (d<duum) {
    d8 = (duum-d)%7;
     if(d8 <= doom){
    day = (doom - d8)% 7;
  
  
     if (day == 0 || day == 7) {
    date = "Sunday";
    println(date);
  } else if (day == 1) {
    date = "Monday";
    println(date);
  } else if (day == 2) {
    date = "Tuesday";
    println(date);
  } else if (day == 3) {
    date = "Wednesday";
    println(date);
  } else if (day == 4) {
    date = "Thursday";
    println(date);
  } else if (day == 5) {
    date = "Friday";
    println(date);
  } else if (day == 6) {
    date = "Saturday";
    println(date);
  }
  }
  if(d8>doom){
    day = (doom - d8) + 7;
    if (day == 0 || day == 7) {
    date = "Sunday";
    println(date);
  } else if (day == 1) {
    date = "Monday";
    println(date);
  } else if (day == 2) {
    date = "Tuesday";
    println(date);
  } else if (day == 3) {
    date = "Wednesday";
    println(date);
  } else if (day == 4) {
    date = "Thursday";
    println(date);
  } else if (day == 5) {
    date = "Friday";
    println(date);
  } else if (day == 6) {
    date = "Saturday";
    println(date);
  }
  }
}
}


may
if (m==5) {
  duum = 9;
  if (d == duum) {
    day = doom;
    if (day == 0 || day == 7) {
      date = "Sunday";
      println(date);
    } else if (day == 1) {
      date = "Monday";
      println(date);
    } else if (day == 2) {
      date = "Tuesday";
      println(date);
    } else if (day == 3) {
      date = "Wednesday";
      println(date);
    } else if (day == 4) {
      date = "Thursday";
      println(date);
    } else if (day == 5) {
      date = "Friday";
      println(date);
    } else if (day == 6) {
      date = "Saturday";
      println(date);
    }
  } else if (d>duum) {
    d8 = (d-duum)%7;
    day = (d8 + doom)%7;

    if (day == 0 || day == 7) {
      date = "Sunday";
      println(date);
    } else if (day == 1) {
      date = "Monday";
      println(date);
    } else if (day == 2) {
      date = "Tuesday";
      println(date);
    } else if (day == 3) {
      date = "Wednesday";
      println(date);
    } else if (day == 4) {
      date = "Thursday";
      println(date);
    } else if (day == 5) {
      date = "Friday";
      println(date);
    } else if (day == 6) {
      date = "Saturday";
      println(date);
    }
  } else if (d<duum) {
    d8 = (duum-d)%7;
    day = (doom - d8)% 7;


    if (day == 0 || day == 7) {
      date = "Sunday";
      println(date);
    } else if (day == 1) {
      date = "Monday";
      println(date);
    } else if (day == 2) {
      date = "Tuesday";
      println(date);
    } else if (day == 3) {
      date = "Wednesday";
      println(date);
    } else if (day == 4) {
      date = "Thursday";
      println(date);
    } else if (day == 5) {
      date = "Friday";
      println(date);
    } else if (day == 6) {
      date = "Saturday";
      println(date);
    }
  }
}


july
if (m==7) {
  duum = 11;
  if (d == duum) {
    day = doom;
    if (day == 0 || day == 7) {
      date = "Sunday";
      println(date);
    } else if (day == 1) {
      date = "Monday";
      println(date);
    } else if (day == 2) {
      date = "Tuesday";
      println(date);
    } else if (day == 3) {
      date = "Wednesday";
      println(date);
    } else if (day == 4) {
      date = "Thursday";
      println(date);
    } else if (day == 5) {
      date = "Friday";
      println(date);
    } else if (day == 6) {
      date = "Saturday";
      println(date);
    }
  } else if (d>duum) {
    d8 = (d-duum)%7;
    day = (d8 + doom)%7;

    if (day == 0 || day == 7) {
      date = "Sunday";
      println(date);
    } else if (day == 1) {
      date = "Monday";
      println(date);
    } else if (day == 2) {
      date = "Tuesday";
      println(date);
    } else if (day == 3) {
      date = "Wednesday";
      println(date);
    } else if (day == 4) {
      date = "Thursday";
      println(date);
    } else if (day == 5) {
      date = "Friday";
      println(date);
    } else if (day == 6) {
      date = "Saturday";
      println(date);
    }
  } else if (d<duum) {
    d8 = (duum-d)%7;
     if(d8 <= doom){
    day = (doom - d8)% 7;
  
  
     if (day == 0 || day == 7) {
    date = "Sunday";
    println(date);
  } else if (day == 1) {
    date = "Monday";
    println(date);
  } else if (day == 2) {
    date = "Tuesday";
    println(date);
  } else if (day == 3) {
    date = "Wednesday";
    println(date);
  } else if (day == 4) {
    date = "Thursday";
    println(date);
  } else if (day == 5) {
    date = "Friday";
    println(date);
  } else if (day == 6) {
    date = "Saturday";
    println(date);
  }
  }
  if(d8>doom){
    day = (doom - d8) + 7;
    if (day == 0 || day == 7) {
    date = "Sunday";
    println(date);
  } else if (day == 1) {
    date = "Monday";
    println(date);
  } else if (day == 2) {
    date = "Tuesday";
    println(date);
  } else if (day == 3) {
    date = "Wednesday";
    println(date);
  } else if (day == 4) {
    date = "Thursday";
    println(date);
  } else if (day == 5) {
    date = "Friday";
    println(date);
  } else if (day == 6) {
    date = "Saturday";
    println(date);
  }
  }
}
}


sept
if (m==9) {
  duum = 5;
  if (d == duum) {
    day = doom;
    if (day == 0 || day == 7) {
      date = "Sunday";
      println(date);
    } else if (day == 1) {
      date = "Monday";
      println(date);
    } else if (day == 2) {
      date = "Tuesday";
      println(date);
    } else if (day == 3) {
      date = "Wednesday";
      println(date);
    } else if (day == 4) {
      date = "Thursday";
      println(date);
    } else if (day == 5) {
      date = "Friday";
      println(date);
    } else if (day == 6) {
      date = "Saturday";
      println(date);
    }
  } else if (d>duum) {
    d8 = (d-duum)%7;
    day = (d8 + doom)%7;

    if (day == 0 || day == 7) {
      date = "Sunday";
      println(date);
    } else if (day == 1) {
      date = "Monday";
      println(date);
    } else if (day == 2) {
      date = "Tuesday";
      println(date);
    } else if (day == 3) {
      date = "Wednesday";
      println(date);
    } else if (day == 4) {
      date = "Thursday";
      println(date);
    } else if (day == 5) {
      date = "Friday";
      println(date);
    } else if (day == 6) {
      date = "Saturday";
      println(date);
    }
  } else if (d<duum) {
    d8 = (duum-d)%7;
     if(d8 <= doom){
    day = (doom - d8)% 7;
  
  
     if (day == 0 || day == 7) {
    date = "Sunday";
    println(date);
  } else if (day == 1) {
    date = "Monday";
    println(date);
  } else if (day == 2) {
    date = "Tuesday";
    println(date);
  } else if (day == 3) {
    date = "Wednesday";
    println(date);
  } else if (day == 4) {
    date = "Thursday";
    println(date);
  } else if (day == 5) {
    date = "Friday";
    println(date);
  } else if (day == 6) {
    date = "Saturday";
    println(date);
  }
  }
  if(d8>doom){
    day = (doom - d8) + 7;
    if (day == 0 || day == 7) {
    date = "Sunday";
    println(date);
  } else if (day == 1) {
    date = "Monday";
    println(date);
  } else if (day == 2) {
    date = "Tuesday";
    println(date);
  } else if (day == 3) {
    date = "Wednesday";
    println(date);
  } else if (day == 4) {
    date = "Thursday";
    println(date);
  } else if (day == 5) {
    date = "Friday";
    println(date);
  } else if (day == 6) {
    date = "Saturday";
    println(date);
  }
  }
}
}


nov
if (m==11) {
  duum = 7;
  if (d == duum) {
    day = doom;
    if (day == 0 || day == 7) {
      date = "Sunday";
      println(date);
    } else if (day == 1) {
      date = "Monday";
      println(date);
    } else if (day == 2) {
      date = "Tuesday";
      println(date);
    } else if (day == 3) {
      date = "Wednesday";
      println(date);
    } else if (day == 4) {
      date = "Thursday";
      println(date);
    } else if (day == 5) {
      date = "Friday";
      println(date);
    } else if (day == 6) {
      date = "Saturday";
      println(date);
    }
  } else if (d>duum) {
    d8 = (d-duum)%7;
    day = (d8 + doom)%7;

    if (day == 0 || day == 7) {
      date = "Sunday";
      println(date);
    } else if (day == 1) {
      date = "Monday";
      println(date);
    } else if (day == 2) {
      date = "Tuesday";
      println(date);
    } else if (day == 3) {
      date = "Wednesday";
      println(date);
    } else if (day == 4) {
      date = "Thursday";
      println(date);
    } else if (day == 5) {
      date = "Friday";
      println(date);
    } else if (day == 6) {
      date = "Saturday";
      println(date);
    }
  } else if (d<duum) {
    d8 = (duum-d)%7;
     if(d8 <= doom){
    day = (doom - d8)% 7;
  
  
     if (day == 0 || day == 7) {
    date = "Sunday";
    println(date);
  } else if (day == 1) {
    date = "Monday";
    println(date);
  } else if (day == 2) {
    date = "Tuesday";
    println(date);
  } else if (day == 3) {
    date = "Wednesday";
    println(date);
  } else if (day == 4) {
    date = "Thursday";
    println(date);
  } else if (day == 5) {
    date = "Friday";
    println(date);
  } else if (day == 6) {
    date = "Saturday";
    println(date);
  }
  }
  if(d8>doom){
    day = (doom - d8) + 7;
    if (day == 0 || day == 7) {
    date = "Sunday";
    println(date);
  } else if (day == 1) {
    date = "Monday";
    println(date);
  } else if (day == 2) {
    date = "Tuesday";
    println(date);
  } else if (day == 3) {
    date = "Wednesday";
    println(date);
  } else if (day == 4) {
    date = "Thursday";
    println(date);
  } else if (day == 5) {
    date = "Friday";
    println(date);
  } else if (day == 6) {
    date = "Saturday";
    println(date);
  }
  }
}
}
