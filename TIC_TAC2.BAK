#include<graphics.h>
#include<stdio.h>
#include<string.h>
#include<stdlib.h>
#include<conio.h>
#include<dos.h>
#include<nagesh.h>
#pragma startup star
#pragma startup loading
void base();
void entery();
void x(const int,const int,const int,const int);
void o(const int,const int);
int chk_plc(const int,const int);
int chk_win(const int,const int*);
void main_game();
int choice,fill[3][3];
void main(void)
{
	int gd=DETECT,gm;
	initgraph(&gd,&gm,"c:\\turboc3\\bgi");
	entery();
	base();
	main_game();
	setcolor(15);
	rectangle(0,40,400,440);
	closegraph();
}
void main_game()
{
	register int count=0,op,j,i;
	int p_t;
	for(i=0;i<3;i++)
	{
		for(j=0;j<3;j++)
		{
			fill[i][j]=0;
		}
	}
	while(count<9)
	{
		op=getch();
		if(op==27)
			count=10;
		if(count%2==0)
		{
			p_t=1;
			op=choice+((int)op-48);
		}
		else
		{
			p_t=2;
			if(choice==10)
				op=20+((int)op-48);
			else if(choice==20)
				op=10+((int)op-48);
		}
		switch(op)
		{
			case 11:    if(chk_plc(0,0))
							{  fill[0][0]=p_t;
								/*1*/   x(20,60,110,150);
								sound(265);
								delay(200);
								count++;
								nosound();
								if(chk_win(1,&p_t))
									count=10;
							}break;
			case 12:		if(chk_plc(0,1))
							{	fill[0][1]=p_t;
								/*2*/   x(155,60,245,150);
								sound(275);
								delay(200);
								count++;
								nosound();
								if(chk_win(2,&p_t))
									count=10;
							}break;
			case 13:		if(chk_plc(0,2))
							{  fill[0][2]=p_t;
								/*3*/	  x(290,60,380,150);
								sound(285);
								delay(200);
								count++;
								nosound();
								if(chk_win(3,&p_t))
									count=10;
							}break;
			case 14:		if(chk_plc(1,0))
							{  fill[1][0]=p_t;
								/*4*/   x(20,195,110,285);
								sound(295);
								delay(200);
								count++;
								nosound();
								if(chk_win(4,&p_t))
									count=10;
							}break;
			case 15:		if(chk_plc(1,1))
							{  fill[1][1]=p_t;
								/*5*/   x(155,195,245,285);
								sound(305);
								delay(200);
								count++;
								nosound();
								if(chk_win(5,&p_t))
									count=10;
							}break;
			case 16:		if(chk_plc(1,2))
							{  fill[1][2]=p_t;
								/*6*/   x(290,195,380,285);
								sound(315);
								delay(200);
								count++;
								nosound();
								if(chk_win(6,&p_t))
									count=10;
							}break;
			case 17:		if(chk_plc(2,0))
							{  fill[2][0]=p_t;
								/*7*/   x(20,330,110,420);
								sound(325);
								delay(200);
								count++;
								nosound();
								if(chk_win(7,&p_t))
									count=10;
							}break;
			case 18:		if(chk_plc(2,1))
							{  fill[2][1]=p_t;
								/*8*/   x(155,330,245,420);
								sound(335);
								delay(200);
								count++;
								nosound();
								if(chk_win(8,&p_t))
									count=10;
							}break;
			case 19:    if(chk_plc(2,2))
							{  fill[2][2]=p_t;
								/*9*/   x(290,330,380,420);
								sound(345);
								delay(200);
								count++;
								nosound();
								if(chk_win(9,&p_t))
									count=10;
							}break;

			case 21:		if(chk_plc(0,0))
							{  fill[0][0]=p_t;
								/*1*/	  o(0,40);
								sound(265);
								delay(200);
								count++;
								nosound();
								if(chk_win(1,&p_t))
									count=10;
							}break;
			case 22:		if(chk_plc(0,1))
							{  fill[0][1]=p_t;
								/*2*/   o(135,40);
								sound(275);
								delay(200);
								count++;
								nosound();
								if(chk_win(2,&p_t))
									count=10;
							}break;
			case 23:		if(chk_plc(0,2))
							{  fill[0][2]=p_t;
								/*3*/   o(270,40);
								sound(285);
								delay(200);
								count++;
								nosound();
								if(chk_win(3,&p_t))
									count=10;
							}break;
			case 24:		if(chk_plc(1,0))
							{  fill[1][0]=p_t;
								/*4*/   o(0,175);
								sound(295);
								delay(200);
								count++;
								nosound();
								if(chk_win(4,&p_t))
									count=10;
							}break;
			case 25:		if(chk_plc(1,1))
							{  fill[1][1]=p_t;
								/*5*/   o(135,175);
								sound(305);
								delay(200);
								count++;
								nosound();
								if(chk_win(5,&p_t))
									count=10;
							}break;
			case 26:		if(chk_plc(1,2))
							{  fill[1][2]=p_t;
								/*6*/   o(270,175);
								sound(315);
								delay(200);
								count++;
								nosound();
								if(chk_win(6,&p_t))
									count=10;
							}break;
			case 27:		if(chk_plc(2,0))
							{  fill[2][0]=p_t;
								/*7*/   o(0,310);
								sound(325);
								delay(200);
								count++;
								nosound();
								if(chk_win(7,&p_t))
									count=10;
							}break;
			case 28:		if(chk_plc(2,1))
							{  fill[2][1]=p_t;
								/*8*/   o(135,310);
								sound(335);
								delay(200);
								count++;
								nosound();
								if(chk_win(8,&p_t))
									count=10;
							}break;
			case 29:		if(chk_plc(2,2))
							{  fill[2][2]=p_t;
								/*9*/   o(270,310);
								sound(345);
								delay(200);
								count++;
								nosound();
								if(chk_win(9,&p_t))
									count=10;
							}break;
		}

	}
	if(count==9)
	{
		setcolor(14);
		settextstyle(2,0,5);
		outtextxy(500,160,"DRAW");
		getch();
	}
}
void entery()
{
	char ch;
	cleardevice();
	while(!(ch==(char)49 || ch==(char)50))
	{
		setcolor(2);
		settextstyle(2,0,8);
		outtextxy(245,70,"PLAYER I");
		setcolor(5);
		settextstyle(2,0,10);
		outtextxy(100,100,"ENTER YOUR CHOICE");
		setcolor(14);
		settextstyle(2,0,7);
		outtextxy(100,160,"PRESS 1 FOR X.");
		outtextxy(100,190,"PRESS 2 FOR O.");
		ch=getch();
		choice=((int)ch-48)*10;
	}
}
void base()
{
	cleardevice();
	setfillstyle(1,1);
	setcolor(1);
/*H1*/	  rectangle(130,40,135,440);
/*H2*/	    rectangle(265,40,270,440);
/*V1*/	      rectangle(0,170,400,175);
/*V2*/      		rectangle(0,305,400,310);
	floodfill(0,0,1);
	floodfill(0,176,1);
	floodfill(136,176,1);
	floodfill(131,171,1);
	floodfill(266,171,1);
	floodfill(131,306,1);
	floodfill(266,306,1);
	setcolor(14);
	settextstyle(3,0,1);
	outtextxy(5,45,"1");
		outtextxy(140,45,"2");
			outtextxy(275,45,"3");
				outtextxy(5,180,"4");
					outtextxy(140,180,"5");
						outtextxy(275,180,"6");
							outtextxy(5,315,"7");
								outtextxy(140,315,"8");
									outtextxy(275,315,"9");
	setcolor(2);
	settextstyle(6,0,1);
	outtextxy(420,450,"PRESS \" ESC KEY \" TO EXIT");
}
void x(const int a,const int b,const int c,const int d)
{
	/* code for "\" */
	setcolor(12);
	setfillstyle(1,12);
	line(a,b+5,c-5,d);
	line(a+5,b,c,d-5);
	line(a,b+5,a+5,b);
	line(c-5,d,c,d-5);
	floodfill(a+6,b+6,12);
	/* code for "/" */
	line(c-5,b,a,d-5);
	line(c,b+5,a+5,d);
	line(c-5,b,c,b+5);
	line(a,d-5,a+5,d);
	floodfill(c-5,b+4,12);
	floodfill(a+5,d-2,12);
}
void o(const int a,const int b)
{
	setcolor(12);
	setfillstyle(1,12);
	circle(a+65,b+65,50);
	circle(a+65,b+65,45);
	floodfill(a+66,b+18,12);
}
int chk_plc(const int a,const int b)
{
	if(fill[a][b]==0)
		return 1;
	return 0;
}
int chk_win(const int ch,const int *p_t)
{  int a=0;
	char *msg;
	switch(ch)
	{
		case 1:     if(fill[0][0]==fill[0][1] && fill[0][0]==fill[0][2])
							a=1;
						if(fill[0][0]==fill[1][0] && fill[0][0]==fill[2][0])
							a=1;
						if(fill[0][0]==fill[1][1] && fill[0][0]==fill[2][2])
							a=1;
					if(a)
					{
						setcolor(14);
						settextstyle(2,0,5);
						sprintf(msg,"PLAYER %d WIN",*p_t);
						outtextxy(500,160,msg);
						getch();
						return 1;
					}break;
		case 2:  	if(fill[0][1]==fill[0][0] && fill[0][1]==fill[0][2])
							a=1;
						if(fill[0][1]==fill[1][1] && fill[0][1]==fill[2][1])
							a=1;
					if(a)
					{
						setcolor(14);
						settextstyle(2,0,5);
						sprintf(msg,"PLAYER %d WIN",*p_t);
						outtextxy(500,160,msg);
						getch();
						return 1;
					}break;
		case 3:  	if(fill[0][2]==fill[0][0] && fill[0][2]==fill[0][1])
							a=1;
						if(fill[0][2]==fill[1][2] && fill[0][2]==fill[2][2])
							a=1;
						if(fill[0][2]==fill[1][1] && fill[0][2]==fill[2][0])
							a=1;
					if(a)
					{
						setcolor(14);
						settextstyle(2,0,3);
						sprintf(msg,"PLAYER %d WIN",*p_t);
						outtextxy(500,160,msg);
						getch();
						return 1;
					}break;
		case 4:  	if(fill[1][0]==fill[1][1] && fill[1][0]==fill[1][2])
							a=1;
						if(fill[1][0]==fill[0][0] && fill[1][0]==fill[2][0])
							a=1;
					if(a)
					{
						setcolor(14);
						settextstyle(2,0,3);
						sprintf(msg,"PLAYER %d WIN",*p_t);
						outtextxy(500,160,msg);
						getch();
						return 1;
					}break;
		case 5:     if(fill[1][1]==fill[1][0] && fill[1][1]==fill[1][2])
							a=1;
						if(fill[1][1]==fill[0][1] && fill[1][1]==fill[2][1])
							a=1;
						if(fill[1][1]==fill[0][0] && fill[1][1]==fill[2][2])
							a=1;
						if(fill[1][1]==fill[0][2] && fill[1][1]==fill[2][0])
							a=1;
					if(a)
					{
						setcolor(14);
						settextstyle(2,0,3);
						sprintf(msg,"PLAYER %d WIN",*p_t);
						outtextxy(500,160,msg);
						getch();
						return 1;
					}break;
		case 6:  	if(fill[1][2]==fill[1][0] && fill[1][2]==fill[1][1])
							a=1;
						if(fill[1][2]==fill[0][2] && fill[1][2]==fill[2][2])
							a=1;
					if(a)
					{
						setcolor(14);
						settextstyle(2,0,3);
						sprintf(msg,"PLAYER %d WIN",*p_t);
						outtextxy(500,160,msg);
						getch();
						return 1;
					}break;
		case 7:     if(fill[2][0]==fill[2][1] && fill[2][0]==fill[2][2])
							a=1;
						if(fill[2][0]==fill[0][0] && fill[2][0]==fill[1][0])
							a=1;
						if(fill[2][0]==fill[0][2] && fill[2][0]==fill[1][1])
							a=1;
					if(a)
					{
						setcolor(14);
						settextstyle(2,0,3);
						sprintf(msg,"PLAYER %d WIN",*p_t);
						outtextxy(500,160,msg);
						getch();
						return 1;
					}break;
		case 8: 		if(fill[2][1]==fill[2][0] && fill[2][1]==fill[2][2])
							a=1;
						if(fill[2][1]==fill[0][1] && fill[2][1]==fill[1][1])
							a=1;
					if(a)
					{
						setcolor(14);
						settextstyle(2,0,3);
						sprintf(msg,"PLAYER %d WIN",*p_t);
						outtextxy(500,160,msg);
						getch();
						return 1;
					}break;
		case 9:  	if(fill[2][2]==fill[2][0] && fill[2][2]==fill[2][1])
							a=1;
						if(fill[2][2]==fill[0][2] && fill[2][2]==fill[1][2])
							a=1;
						if(fill[2][2]==fill[0][0] && fill[2][2]==fill[1][1])
							a=1;
					if(a)
					{
						setcolor(14);
						settextstyle(2,0,3);
						sprintf(msg,"PLAYER %d WIN",*p_t);
						outtextxy(500,160,msg);
						getch();
						return 1;
					}break;
	}
	return 0;
}