#include <stdlib.h>
#include<math.h>
#include <glut.h>
float i = .2;
int j = 0, k = 0, l = 0;
GLfloat vertices[][3] =
{
	{ -42.53, 0, 57.45 }, { -13.14, -40.45, 57.45 },
	{ 34.41, -25, 57.45 }, { 34.41, 25, 57.45 },
	{ -13.41, 40.45, 57.45 }, { -65.50, 0, 13 },
	{ -20, -60, 13 }, { 52.89, -38.47, 13 },
	{ 52.89, 38.47, 13 }, { -20.30, 62.25, 13 },
	{ -52.89, -38.47, -13 }, { 20, -60, -13 },
	{ 65.50, 0, -13 }, { 20.30, 62.25, -13 },
	{ -52.89, 38.47, -13 }, { -34.41, -25, -57.45 },
	{ 13.14, -40.45, -57.45 }, { 42.53, 0, -57.45 },
	{ 13.14, 40.45, -57.45 }, { -34.41, 25, -57.45 },
	{ -76.08, -55.28, 46.08 }, { 29.08, -89.49, 46.08 },
	{ 94.05, 0, 46.08 }, { 29.08, 89.49, 46.08 },
	{ -76.08, 55.28, 46.08 }, { -29.09, -89.53, -46.08 },
	{ 76.08, -55.28, -46.08 }, { 76.08, 55.28, -46.08 },
	{ -29.08, 89.49, -46.08 }, { -94.05, 0, -46.08 },
	{ 0, 0, 107.42 }, { 0, 0, -107.42 },
	{ -50.0, -50.0, -50.0 }, { 50.0, -50.0, -50.0 },
	{ 50.0, 50.0, -50.0 }, { -50.0, 50.0, -50.0 },
	{ -50.0, -50.0, 50.0 }, { 50.0, -50.0, 50.0 },
	{ 50.0, 50.0, 50.0 }, { -50.0, 50.0, 50.0 },
	{ 0, 0, 100 }, { 0, 0, -100 },
	{ -100, 0, 0 }, { 0, 100, 0 },
	{ 100, 0, 0 }, { 0, -100, 0 }
};

GLfloat colors[][3] =
{
	{ 0.0, 0.0, 1.0 }, { 0.0, 1.0, 0.0 },
	{ 0.5, 1.0, 0.0 }, { 0.0, 1.0, 1.0 }, { 1.0, 0.0, 0.0 },
	{ 1.0, 0.0, 1.0 }, { 1.0, 1.0, 0.0 }, { 0.5, 1.0, 1.0 },
	{ 1.0, 1.0, 0.50 }, { 0.50, 0.30, 1.0 }, { 0.0, 1.0, .50 },
	{ 1.0, 0.0, 0.0 }, { 0.0, 1.0, .50 }, { 1.0, 0.0, 0.0 },
	{ 1.0, 1.0, 0.0 }, { 0.0, 1.0, 0.0 }, { 0.0, 0.0, 1.0 },
	{ 1.0, 0.0, 1.0 }, { 1.0, 1.0, 1.0 }, { 0.0, 1.0, 1.0 },
	{ 1.0, 1.0, 1.0 }, { 0.0, 1.0, 1.0 }, { 0.0, 1.0, .50 },
	{ 1.0, 0.0, 0.0 }, { 0.0, 1.0, .50 }, { 1.0, 0.0, 0.0 },
	{ 1.0, 1.0, 0.0 }, { 0.0, 1.0, 0.0 }, { 0.0, 0.0, 1.0 },
	{ 1.0, 0.0, 1.0 }, { 1.0, 1.0, 1.0 }, { 0.0, 1.0, 1.0 },
	{ 1.0, 1.0, 1.0 }, { 0.0, 1.0, 1.0 }, { 0.0, 1.0, .50 },
	{ 1.0, 0.0, 0.0 }, { 0.0, 1.0, .50 }, { 1.0, 0.0, 0.0 },
	{ 1.0, 1.0, 0.0 }, { 0.0, 1.0, 0.0 }, { 0.0, 0.0, 1.0 },
	{ 1.0, 0.0, 1.0 }, { 1.0, 1.0, 1.0 }, { 0.0, 1.0, 1.0 },
	{ 1.0, 1.0, 1.0 }, { 0.0, 1.0, 1.0 }, { 0.0, 1.0, .50 },
	{ 1.0, 0.0, 0.0 }
};
GLfloat normals[][3] = { { 0.0, 0.0, 0.0 }, { 0.0, 0.0, 0.0 }, { 0.0, 0.0, 0.0 } };
void polygon(int a, int b, int c)
{
	glBegin(GL_POLYGON);
	glColor3fv(colors[a]);
	glNormal3fv(normals[a]);
	glVertex3fv(vertices[a]);
	glColor3fv(colors[b]);
	glNormal3fv(normals[b]);
	glVertex3fv(vertices[b]);
	glColor3fv(colors[c]);
	glNormal3fv(normals[c]);
	glVertex3fv(vertices[c]);

	glEnd();
}

void pent0()
{
	polygon(1, 0, 31);
	polygon(2, 1, 31);
	polygon(3, 2, 31);
	polygon(4, 3, 31);
	polygon(0, 4, 31);
}
void pent1()
{
	polygon(15, 16, 30);
	polygon(16, 17, 30);
	polygon(17, 18, 30);
	polygon(18, 19, 30);
	polygon(19, 15, 30);
}
void pent2()
{
	polygon(1, 0, 27);
	polygon(0, 5, 27);
	polygon(5, 10, 27);
	polygon(10, 6, 27);
	polygon(6, 1, 27);
}
void pent3()
{
	polygon(2, 1, 28);
	polygon(1, 6, 28);
	polygon(6, 11, 28);
	polygon(11, 7, 28);
	polygon(7, 2, 28);
}
void pent4()
{
	polygon(3, 2, 29);
	polygon(2, 7, 29);
	polygon(7, 12, 29);
	polygon(12, 8, 29);
	polygon(8, 3, 29);
}
void pent5()
{
	polygon(4, 3, 25);
	polygon(3, 8, 25);
	polygon(8, 13, 25);
	polygon(13, 9, 25);
	polygon(9, 4, 25);
}
void pent6()
{
	polygon(0, 4, 26);
	polygon(4, 9, 26);
	polygon(9, 14, 26);
	polygon(14, 5, 26);
	polygon(5, 0, 26);
}
void pent7()
{
	polygon(0, 1, 27);
	polygon(0, 5, 27);
	polygon(5, 10, 27);
	polygon(10, 6, 27);
	polygon(6, 1, 27);
}
void pent8()
{
	polygon(15, 16, 23);
	polygon(16, 11, 23);
	polygon(11, 6, 23);
	polygon(6, 10, 23);
	polygon(10, 15, 23);
}
void pent9()
{
	polygon(16, 17, 24);
	polygon(17, 12, 24);
	polygon(12, 7, 24);
	polygon(7, 11, 24);
	polygon(11, 16, 24);
}
void pent10()
{
	polygon(17, 18, 20);
	polygon(18, 13, 20);
	polygon(13, 8, 20);
	polygon(8, 12, 20);
	polygon(12, 17, 20);
}
void pent11()
{
	polygon(18, 19, 21);
	polygon(19, 14, 21);
	polygon(14, 9, 21);
	polygon(9, 13, 21);
	polygon(13, 18, 21);
}
void pent12()
{
	polygon(19, 15, 22);
	polygon(15, 10, 22);
	polygon(10, 5, 22);
	polygon(5, 14, 22);
	polygon(14, 19, 22);
}
void cube1()
{
	polygon(32, 33, 40);
	polygon(33, 34, 40);
	polygon(34, 35, 40);
	polygon(35, 32, 40);
}
void cube2()
{
	polygon(37, 33, 42);
	polygon(33, 34, 42);
	polygon(34, 38, 42);
	polygon(37, 38, 42);
}
void cube3()
{
	polygon(36, 39, 44);
	polygon(39, 35, 44);
	polygon(35, 32, 44);
	polygon(32, 36, 44);
}
void cube4()
{
	polygon(33, 32, 43);
	polygon(33, 37, 43);
	polygon(36, 37, 43);
	polygon(36, 32, 43);
}
void cube5()
{
	polygon(36, 37, 41);
	polygon(37, 38, 41);
	polygon(38, 39, 41);
	polygon(39, 36, 41);
}
void cube6()
{
	polygon(34, 35, 45);
	polygon(35, 39, 45);
	polygon(39, 38, 45);
	polygon(38, 34, 45);
}
static GLfloat theta[] = { 0.10, 0.10, 0.10 };
static GLint axis = 2;

void display(void)
{
	glClear(GL_COLOR_BUFFER_BIT | GL_DEPTH_BUFFER_BIT);
	glLoadIdentity();

	glRotatef(theta[0], 1.0, 0.0, 0.0);
	glRotatef(theta[1], 0.0, 0.0, 1.0);
	glRotatef(theta[2], 0.0, 1.0, 0.0);
	if (j <= 0)
	{
		if (l>0)
			cube1();
		if (l>1)
			cube5();
		if (l>2)
			cube2();
		if (l>3)
			cube3();
		if (l>4)
			cube4();
		if (l>5)
			cube6();
	}

	else
	{
		if (j>0)
			pent0();
		if (j>1)
			pent1();
		if (j>2)
			pent2();
		if (j>3)
			pent3();
		if (j>4)
			pent4();
		if (j>5)
			pent5();
		if (j>6)
			pent6();
		if (j>7)
			pent7();
		if (j>8)
			pent8();
		if (j>9)
			pent9();
		if (j>10)
			pent10();
		if (j>11)
			pent11();
		if (j >= 11)
			pent12();

	}

	glFlush();
	glutSwapBuffers();
}

void spinner()
{

	theta[axis] = theta[axis] + 3.5*sin(i);
	if (k == 250 || sin(i) == 0)
	{
		axis = (axis + 1) % 3;
		if (k == 250 || (sin(i) >= .5998 && sin(i) <= 1))
			k = 0;
	}
	if (theta[axis] >= 360.0)
	{
		theta[axis] -= 360.0;
	}
	i += .005;
	if (i>6.2830)
		i = 0;
	k++;
	glutPostRedisplay();
}

void mouse(int btn, int state, int x, int y)
{

	if (j != 12 && l != 7)
		if (btn == GLUT_LEFT_BUTTON && state == GLUT_DOWN)
		{
			if (l<6)
				l++;
			else
				j++;
		}

	if (btn == GLUT_MIDDLE_BUTTON && state == GLUT_DOWN) axis = 1;

	if (btn == GLUT_RIGHT_BUTTON && state == GLUT_DOWN)
	{
		if (j>0)
			j--;
		else if (l>0)
			l--;
	}
}

void myReshape(int w, int h)
{
	glViewport(0, 0, w, h);
	glMatrixMode(GL_PROJECTION);
	glLoadIdentity();
	if (w <= h)
		glOrtho(-150.0, 150.0, -150.0 * (GLfloat)h / (GLfloat)w,
		150.0 * (GLfloat)h / (GLfloat)w, -750.0, 750.0);
	else
		glOrtho(-150.0 * (GLfloat)w / (GLfloat)h,
		150.0 * (GLfloat)w / (GLfloat)h, -150.0, 150.0, -750.0, 750.0);
	glMatrixMode(GL_MODELVIEW);
}

void
main(int argc, char **argv)
{
	glutInit(&argc, argv);
	glutInitDisplayMode(GLUT_DOUBLE | GLUT_RGB | GLUT_DEPTH);
	glutInitWindowSize(1250, 750);
	glutCreateWindow("Dancing Star");
	glutReshapeFunc(myReshape);
	glutDisplayFunc(display);
	glutIdleFunc(spinner);
	glutMouseFunc(mouse);
	glEnable(GL_DEPTH_TEST);
	glutMainLoop();
}
