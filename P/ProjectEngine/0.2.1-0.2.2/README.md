# Comparing `tmp/projectengine-0.2.1.tar.gz` & `tmp/projectengine-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "projectengine-0.2.1.tar", last modified: Thu May  2 16:07:57 2024, max compression
+gzip compressed data, was "projectengine-0.2.2.tar", last modified: Wed May  8 11:37:06 2024, max compression
```

## Comparing `projectengine-0.2.1.tar` & `projectengine-0.2.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-05-02 16:07:57.871283 projectengine-0.2.1/
--rw-rw-rw-   0        0        0      207 2024-05-02 16:07:57.866710 projectengine-0.2.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-05-02 16:07:57.790459 projectengine-0.2.1/ProjectEngine/
--rw-rw-rw-   0        0        0      998 2024-02-08 09:07:33.000000 projectengine-0.2.1/ProjectEngine/Shaders.py
--rw-rw-rw-   0        0        0       30 2024-05-01 13:40:35.000000 projectengine-0.2.1/ProjectEngine/__init__.py
--rw-rw-rw-   0        0        0    16094 2024-05-01 14:21:16.000000 projectengine-0.2.1/ProjectEngine/classes.py
--rw-rw-rw-   0        0        0      744 2024-04-30 14:14:34.000000 projectengine-0.2.1/ProjectEngine/main.py
-drwxrwxrwx   0        0        0        0 2024-05-02 16:07:57.859292 projectengine-0.2.1/ProjectEngine.egg-info/
--rw-rw-rw-   0        0        0      207 2024-05-02 16:07:57.000000 projectengine-0.2.1/ProjectEngine.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      290 2024-05-02 16:07:57.000000 projectengine-0.2.1/ProjectEngine.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-02 16:07:57.000000 projectengine-0.2.1/ProjectEngine.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2024-05-02 16:07:57.000000 projectengine-0.2.1/ProjectEngine.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2024-05-02 16:07:57.000000 projectengine-0.2.1/ProjectEngine.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-02 16:07:57.873293 projectengine-0.2.1/setup.cfg
--rw-rw-rw-   0        0        0      332 2024-05-02 16:07:31.000000 projectengine-0.2.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-08 11:37:06.018996 projectengine-0.2.2/
+-rw-rw-rw-   0        0        0      292 2024-05-08 11:37:06.013807 projectengine-0.2.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-08 11:37:05.921666 projectengine-0.2.2/ProjectEngine/
+-rw-rw-rw-   0        0        0      998 2024-02-08 09:07:33.000000 projectengine-0.2.2/ProjectEngine/Shaders.py
+-rw-rw-rw-   0        0        0       30 2024-05-03 09:21:15.000000 projectengine-0.2.2/ProjectEngine/__init__.py
+-rw-rw-rw-   0        0        0    17436 2024-05-05 21:29:25.000000 projectengine-0.2.2/ProjectEngine/classes.py
+-rw-rw-rw-   0        0        0     1107 2024-05-04 08:36:34.000000 projectengine-0.2.2/ProjectEngine/main.py
+drwxrwxrwx   0        0        0        0 2024-05-08 11:37:06.006427 projectengine-0.2.2/ProjectEngine.egg-info/
+-rw-rw-rw-   0        0        0      292 2024-05-08 11:37:05.000000 projectengine-0.2.2/ProjectEngine.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      290 2024-05-08 11:37:05.000000 projectengine-0.2.2/ProjectEngine.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-08 11:37:05.000000 projectengine-0.2.2/ProjectEngine.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       26 2024-05-08 11:37:05.000000 projectengine-0.2.2/ProjectEngine.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2024-05-08 11:37:05.000000 projectengine-0.2.2/ProjectEngine.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-08 11:37:06.021002 projectengine-0.2.2/setup.cfg
+-rw-rw-rw-   0        0        0      433 2024-05-08 11:34:48.000000 projectengine-0.2.2/setup.py
```

### Comparing `projectengine-0.2.1/ProjectEngine/Shaders.py` & `projectengine-0.2.2/ProjectEngine/Shaders.py`

 * *Files identical despite different names*

### Comparing `projectengine-0.2.1/ProjectEngine/classes.py` & `projectengine-0.2.2/ProjectEngine/classes.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,23 +1,26 @@
 import pygame
 from pygame.locals import *
 
 from OpenGL.GL import *
 from OpenGL.GLU import *
 
-from objloader.objloader import *
+#from objloader.objloader import *
+from objloader import *
 
 import threading
 #import winsound
 #from Shaders import *
 
-def ThreadingFunc(func):
-	print("Threaded")
-	#threading.Thread(target=lambda:func()).start()
-	func()
+def threaded(fn):
+    def wrapper(*args, **kwargs):
+        threading.Thread(target=fn, args=args, kwargs=kwargs).start()
+    return wrapper
+def Debug(string):
+	print(string)
 class RigidBody3:
 	def __init__(self):
 		pass
 class Render:
 	VERTICIES = 1
 	OBJ = 2
 class DRAWTYPE:
@@ -29,15 +32,23 @@
 		self.win = None
 		self.events = []
 		self.pressed = {'A1':False,'A': False,'B': False,'C': False,'D': False,'E': False,'F': False,'G': False,'H': False,'I': False,'J': False,'K': False,'L': False,'M': False,'N': False,'O': False,'P': False,'Q': False,'R': False,'S': False,'T': False,'U': False,'V': False,'W': False,'X': False,'Y': False,'Z': False}
 	def addWin(self,w):
 		self.win = w
 	def addEvents(self,e):
 		self.events = e
-	def update(self): # make this threaded
+	def updateRework(self,key):
+		x = False
+		ldict = {}
+		exec(f"x = pygame.key.get_pressed()[pygame.K_{key.lower()}]",{'x':x,'pygame':pygame},ldict)
+		return ldict['x']
+	#@threaded                                                          
+	def update(self,key):
+		return self.updateRework(key)
+	def Update(self): # make this threaded
 		#print("Update")
 		#print(self.pressed)
 		for i in self.pressed.keys():
 			self.pressed[i] = False
 		i = pygame.key.get_pressed()
 		#print(i[pygame.K_a])
 		#if True:
@@ -256,15 +267,15 @@
 					self.pressed["Y"] = False
 				if i.key == pygame.K_z:
 					self.pressed["Z"] = False'''
 class Shapes:
 	def Cube():
 		verticies = ((1, -1, -1),(1, 1, -1),(-1, 1, -1),(-1, -1, -1),(1, -1, 1),(1, 1, 1),(-1, -1, 1),(-1, 1, 1))
 		edges = ((0,1),(0,3),(0,4),(2,1),(2,3),(2,7),(6,3),(6,4),(6,7),(5,1),(5,4),(5,7))
-		triangles = ( (0,0,0),(0,1,0),(1,0,0), (0,1,0),(1,1,0),(1,0,0), (0,0,0),(0,1,0),(0,0,1), (0,1,1),(0,1,0),(0,0,1), (0,1,0),(1,1,0),(0,1,1), (0,1,1),(1,1,1),(1,1,0) )
+		triangles = ( (0,0,0),(0,1,0),(1,0,0), (0,1,0),(1,1,0),(1,0,0), (0,0,0),(0,1,0),(0,0,1), (0,1,1),(0,1,0),(0,0,1), (0,1,0),(1,1,0),(0,1,1), (0,1,1),(1,1,1),(1,1,0), (0,0,1),(1,0,1),(0,1,1), (0,1,1),(1,1,1),(1,0,1), (1,0,0),(1,1,0),(1,0,1), (1,1,0),(1,1,1),(1,0,1), (0,0,0),(1,0,0),(1,0,1), (0,0,0),(0,0,1),(1,0,1) )
 		#vao = glGenVertexArrays(1)
 		#glBindVertexArray(self.vao)
 		#vbo = glGenBuffers(1)
 		#glBindBuffer(GL_ARRAY_BUFFER,vbo)
 		#glBufferData(GL_ARRAY_BUFFER,verticies.nbytes,GL_STATIC_DRAW)
 		#glEnableVertexAttribArray(0)
 		#glVertexAttribPointer(0,3,GL_FLOAT,GL_FALSE,32, ctypes.c_void_p(0))
@@ -286,14 +297,15 @@
 		self.rotation = [0,0,0]
 		self.active = True
 		self.move = [0,0,0]
 		self.colour = colour
 		self.alpha = alpha
 		self.type = Type
 		self.debug = False
+		self.physicsModel = None
 		#self.shader = Shader()
 		#glUseProgram(self.shader)
 		#glUniformli(glGetUniformLocation(self.shader,"imageTexture"),0)
 		
 	def rotate(self,vector):
 		self.rotation[0] += vector[0]
 		self.rotation[1] += vector[1]
@@ -302,14 +314,15 @@
 			if i >= 360:
 				i = 0
 	def setColour(self,colour,alpha=255):
 		self.colour = colour
 		self.alpha = alpha
 	def scale(self,by):
 		self.verts["VERT"] = UsefulFunctions.scaleVerticies(by,self.verts["VERT"])
+		self.verts["TRI"] = UsefulFunctions.scaleVerticies(by,self.verts["TRI"])
 	def transform(self,vector):
 		self.move[0] += vector[0]
 		self.move[1] += vector[1]
 		self.move[2]= vector[2]
 	def render(self,cam):
 		glTranslatef(-cam.location[0],-cam.location[1],-cam.location[2])
 		glPushMatrix()
@@ -318,33 +331,34 @@
 		#	#print("HERE")
 		#	glEnable(GL_TEXTURE_2D)
 		#	glBindTexture(GL_TEXTURE_2D,self.texture.texture)
 		glRotatef(self.rotation[0],1,0,0)
 		glRotatef(self.rotation[1],0,1,0)
 		glRotatef(self.rotation[2],0,0,1)
 		glTranslatef(self.move[0],self.move[1],self.move[2])
+		
 		if self.type == DRAWTYPE.WIREFRAME:
 			glBegin(GL_LINES)
 			x = UsefulFunctions.scaleVerticies(self.shape,self.verts["VERT"])
 			for edge in self.verts["EDGE"]:
-				if self.debug == True: print(edge)
+				if self.debug == True: threading.Thread(target=lambda: Debug(edge)).start()
 				for vertex in edge:
-					if self.debug == True: print(vertex)
+					if self.debug == True: threading.Thread(target=lambda: Debug(vertex)).start()
 					glVertex3fv(x[vertex])
 		elif self.type == DRAWTYPE.SOLID:
 			glBegin(GL_TRIANGLES)
 			x = UsefulFunctions.scaleVerticies(self.shape,self.verts["TRI"])
-			print(x)
-			if self.debug == True: print(x)
+			if self.debug == True: threading.Thread(target=lambda: Debug(x)).start()
+			#if self.debug == True: print(x)
 			#for edge in self.verts["TRI"]:
 			for edge in x:
-				if self.debug == True: print(edge)
+				if self.debug == True: threading.Thread(target=lambda: Debug(edge)).start()
 				glVertex3f(edge[0],edge[1],edge[2])
 				for vertex in edge:
-					if self.debug == True: print(vertex)
+					if self.debug == True: threading.Thread(target=lambda: Debug(vertex)).start()
 					
 					#glVertex3fv(x[vertex])
 					#glVertex3f(vertex)
 		else:
 			glBegin(GL_LINES)
 		
 		glColor(round(self.colour[0]/255,2),round(self.colour[1]/255,2),round(self.colour[2]/255),round(self.alpha/255,2))
@@ -353,14 +367,16 @@
 		glPopMatrix()
 		glTranslatef(cam.location[0],cam.location[1],cam.location[2])
 	def toggleActive(self,to=None):
 		if to:
 			self.active = to
 			return
 		self.active = not(self.active)
+	def apply(self,physics):
+		self.physicsModel = physics
 class UsefulFunctions:
 	def scaleVerticies(scale,verticies, triangles=True):  # Take into Classes
 		'''if triangles == True:
 			pass
 			x = []
 			for i in verticies:
 				toAdd = []
@@ -460,28 +476,35 @@
 		glTranslatef(0.0,0.0,-50.0)
 		self.isRunning = False
 		self.objects = []
 		self.fpsgoal = fpsgoal
 		self.clock = pygame.time.Clock()
 		self.camera = None
 		self.keyboard_reader = None
+		self.isdebugging = False
+	def toggleIsdebugging(self,classediting=False):
+		if classediting == False: self.isdebugging = not(self.isdebugging)
+		if self.isdebugging:
+			for obj in self.objects:
+				obj.debug = True
 	def addKeyboardReader(self,k):
 		self.keyboard_reader = k
 		self.keyboard_reader.addWin(self)
 	def playsound(self,filename):
 		sound = pygame.mixer.Sound(filename)
 		sound.play()
 	def run(self,func=None):
 		self.isRunning = True
 		while 1:
 			if self.keyboard_reader:
-				threading.Thread(target=self.keyboard_reader.update).start()
+				#threading.Thread(target=self.keyboard_reader.update).start()
 				#self.keyboard_reader.update()
-				self.keyboard_reader.addEvents(pygame.event.get())
+				#self.keyboard_reader.addEvents(pygame.event.get())
 				#print(pygame.key.get_pressed())
+				pass
 			for event in pygame.event.get():
 				#if self.keyboard_reader:
 				#	
 				if event.type == pygame.QUIT:
 					pygame.quit()
 					quit()
 			glClear(GL_COLOR_BUFFER_BIT|GL_DEPTH_BUFFER_BIT)
@@ -496,16 +519,21 @@
 		#glTranslatef(-self.camera.location[0],-self.camera.location[1],-self.camera.location[2])
 		for i in self.objects:
 			if i.active == True:
 				i.render(cam)
 		#glTranslatef(self.camera.location[0],self.camera.location[1],self.camera.location[2])
 	def addObj(self,obj):
 		self.objects.append(obj)
+		self.toggleIsdebugging(classediting=True)
 	def setCamera(self,c):
 		self.camera = c
+	def tick_physics(self):
+		for i in self.objects:
+			if i.physicsModel:
+				i.move[1] -= i.physicsModel.speed
 if __name__ == "__main__":
 	pygame.init()
 	display = (800,600)
 	pygame.display.set_mode(display, DOUBLEBUF|OPENGL)
 	clock = pygame.time.Clock()
 	gluPerspective(45, (display[0]/display[1]), 0.1, 75)
 	glTranslatef(0.0,0.0, -50)
```

