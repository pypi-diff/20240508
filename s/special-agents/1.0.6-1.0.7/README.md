# Comparing `tmp/special_agents-1.0.6.tar.gz` & `tmp/special_agents-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "special_agents-1.0.6.tar", last modified: Tue May  7 12:10:54 2024, max compression
+gzip compressed data, was "special_agents-1.0.7.tar", last modified: Tue May  7 22:26:26 2024, max compression
```

## Comparing `special_agents-1.0.6.tar` & `special_agents-1.0.7.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxrwx   0        0        0        0 2024-05-07 12:10:54.164256 special_agents-1.0.6/
--rw-rw-rw-   0        0        0     4307 2024-05-07 11:00:25.000000 special_agents-1.0.6/CONTRIBUTING.md
--rw-rw-rw-   0        0        0     1065 2024-05-06 10:26:56.000000 special_agents-1.0.6/LICENSE
--rw-rw-rw-   0        0        0       47 2024-05-06 13:58:26.000000 special_agents-1.0.6/MANIFEST.in
--rw-rw-rw-   0        0        0     4452 2024-05-07 12:10:54.161767 special_agents-1.0.6/PKG-INFO
--rw-rw-rw-   0        0        0     3910 2024-05-07 11:27:20.000000 special_agents-1.0.6/README.md
--rw-rw-rw-   0        0        0       14 2024-05-07 11:14:15.000000 special_agents-1.0.6/requirements.txt
--rw-rw-rw-   0        0        0       42 2024-05-07 12:10:54.164256 special_agents-1.0.6/setup.cfg
--rw-rw-rw-   0        0        0     1026 2024-05-07 12:10:42.000000 special_agents-1.0.6/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-07 12:10:54.037389 special_agents-1.0.6/src/
-drwxrwxrwx   0        0        0        0 2024-05-07 12:10:54.085035 special_agents-1.0.6/src/special_agents/
--rw-rw-rw-   0        0        0     1600 2024-05-07 12:10:17.000000 special_agents-1.0.6/src/special_agents/Agent.py
--rw-rw-rw-   0        0        0       88 2024-05-07 12:04:20.000000 special_agents-1.0.6/src/special_agents/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-07 12:10:54.155823 special_agents-1.0.6/src/special_agents/agents/
--rw-rw-rw-   0        0        0     5205 2024-05-07 12:06:28.000000 special_agents-1.0.6/src/special_agents/agents/ContentCreator.py
--rw-rw-rw-   0        0        0     4221 2024-05-07 12:06:33.000000 special_agents-1.0.6/src/special_agents/agents/FullStackDeveloper.py
--rw-rw-rw-   0        0        0     6063 2024-05-07 12:06:37.000000 special_agents-1.0.6/src/special_agents/agents/ProductManager.py
--rw-rw-rw-   0        0        0       95 2024-05-07 11:09:17.000000 special_agents-1.0.6/src/special_agents/agents/__init__.py
--rw-rw-rw-   0        0        0      310 2024-05-06 21:25:26.000000 special_agents-1.0.6/src/special_agents/config.py
--rw-rw-rw-   0        0        0     4428 2024-05-07 12:08:47.000000 special_agents-1.0.6/src/special_agents/utils.py
-drwxrwxrwx   0        0        0        0 2024-05-07 12:10:54.159226 special_agents-1.0.6/src/special_agents.egg-info/
--rw-rw-rw-   0        0        0     4452 2024-05-07 12:10:53.000000 special_agents-1.0.6/src/special_agents.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      570 2024-05-07 12:10:54.000000 special_agents-1.0.6/src/special_agents.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-07 12:10:53.000000 special_agents-1.0.6/src/special_agents.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       15 2024-05-07 12:10:53.000000 special_agents-1.0.6/src/special_agents.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2024-05-07 12:10:53.000000 special_agents-1.0.6/src/special_agents.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-07 22:26:26.837930 special_agents-1.0.7/
+-rw-rw-rw-   0        0        0     4307 2024-05-07 11:00:25.000000 special_agents-1.0.7/CONTRIBUTING.md
+-rw-rw-rw-   0        0        0     1065 2024-05-06 10:26:56.000000 special_agents-1.0.7/LICENSE
+-rw-rw-rw-   0        0        0       47 2024-05-06 13:58:26.000000 special_agents-1.0.7/MANIFEST.in
+-rw-rw-rw-   0        0        0     8185 2024-05-07 22:26:26.837930 special_agents-1.0.7/PKG-INFO
+-rw-rw-rw-   0        0        0     7441 2024-05-07 22:22:28.000000 special_agents-1.0.7/README.md
+-rw-rw-rw-   0        0        0       14 2024-05-07 11:14:15.000000 special_agents-1.0.7/requirements.txt
+-rw-rw-rw-   0        0        0       42 2024-05-07 22:26:26.837930 special_agents-1.0.7/setup.cfg
+-rw-rw-rw-   0        0        0      939 2024-05-07 22:25:39.000000 special_agents-1.0.7/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-07 22:26:26.731569 special_agents-1.0.7/src/
+drwxrwxrwx   0        0        0        0 2024-05-07 22:26:26.785876 special_agents-1.0.7/src/special_agents/
+-rw-rw-rw-   0        0        0     1563 2024-05-07 22:23:13.000000 special_agents-1.0.7/src/special_agents/Agent.py
+-rw-rw-rw-   0        0        0       85 2024-05-07 19:55:13.000000 special_agents-1.0.7/src/special_agents/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-07 22:26:26.837930 special_agents-1.0.7/src/special_agents/agents/
+-rw-rw-rw-   0        0        0     5103 2024-05-07 19:55:13.000000 special_agents-1.0.7/src/special_agents/agents/ContentCreator.py
+-rw-rw-rw-   0        0        0     4149 2024-05-07 19:55:13.000000 special_agents-1.0.7/src/special_agents/agents/FullStackDeveloper.py
+-rw-rw-rw-   0        0        0     5938 2024-05-07 19:55:13.000000 special_agents-1.0.7/src/special_agents/agents/ProductManager.py
+-rw-rw-rw-   0        0        0       95 2024-05-07 11:09:17.000000 special_agents-1.0.7/src/special_agents/agents/__init__.py
+-rw-rw-rw-   0        0        0      310 2024-05-06 21:25:26.000000 special_agents-1.0.7/src/special_agents/config.py
+-rw-rw-rw-   0        0        0     4330 2024-05-07 19:55:13.000000 special_agents-1.0.7/src/special_agents/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-07 22:26:26.837930 special_agents-1.0.7/src/special_agents.egg-info/
+-rw-rw-rw-   0        0        0     8185 2024-05-07 22:26:26.000000 special_agents-1.0.7/src/special_agents.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      570 2024-05-07 22:26:26.000000 special_agents-1.0.7/src/special_agents.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-07 22:26:26.000000 special_agents-1.0.7/src/special_agents.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       15 2024-05-07 22:26:26.000000 special_agents-1.0.7/src/special_agents.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2024-05-07 22:26:26.000000 special_agents-1.0.7/src/special_agents.egg-info/top_level.txt
```

### Comparing `special_agents-1.0.6/CONTRIBUTING.md` & `special_agents-1.0.7/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `special_agents-1.0.6/LICENSE` & `special_agents-1.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `special_agents-1.0.6/setup.py` & `special_agents-1.0.7/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,30 +1,29 @@
-from setuptools import setup, find_packages
-
-with open("README.md", "r", encoding="utf-8") as fh:
-    long_description = fh.read()
-    
-with open("requirements.txt", "r", encoding="utf-8") as f:
-    req = f.readlines()
-req = [x.strip() for x in req if x.strip()]
-
-setup(
-    name="special-agents", 
-    version="1.0.6",
-    author="Ihab Tag",
-    author_email="contact@ihabtag.com",
-    description="An Open-source Library for pre-defined LLM powered specialized agents",
-    long_description=long_description,
-    long_description_content_type="text/markdown",
-    url="https://github.com/IhabTag/special-agents",
-    # packages=setuptools.find_packages(),
-    classifiers=[
-        "Programming Language :: Python :: 3",
-        "License :: OSI Approved :: MIT License",
-        "Operating System :: OS Independent",
-    ],
-    package_dir={"": "src"},
-    packages = ['special_agents', 'special_agents.agents'],
-    python_requires='>=3.6',
-    license='MIT license',
-    install_requires=req
+from setuptools import setup
+
+with open("README.md", "r", encoding="utf-8") as fh:
+    long_description = fh.read()
+    
+with open("requirements.txt", "r", encoding="utf-8") as f:
+    req = f.readlines()
+req = [x.strip() for x in req if x.strip()]
+
+setup(
+    name="special-agents", 
+    version="1.0.7",
+    author="Ihab Tag",
+    author_email="contact@ihabtag.com",
+    description="An Open-source Library for pre-defined LLM powered specialized agents",
+    long_description=long_description,
+    long_description_content_type="text/markdown",
+    url="https://github.com/IhabTag/special-agents",
+    classifiers=[
+        "Programming Language :: Python :: 3",
+        "License :: OSI Approved :: MIT License",
+        "Operating System :: OS Independent",
+    ],
+    package_dir={"": "src"},
+    packages = ['special_agents', 'special_agents.agents'],
+    python_requires='>=3.6',
+    license='MIT license',
+    install_requires=req
 )
```

### Comparing `special_agents-1.0.6/src/special_agents/Agent.py` & `special_agents-1.0.7/src/special_agents/Agent.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,42 +1,42 @@
-
-from .utils import *
-from .config import *
-
-class Agent:
-
-    def __init__(self, role= '', 
-                 competencies='', 
-                 capabilities= '',
-                 tone= '',
-                 lang= '',
-                 extra_instructions= '',
-                 openai_api_key: str=AGENTS_OPENAI_API_KEY, 
-                 model: str=AGENTS_MODEL,
-                 temperature: float=AGENTS_MODEL_TEMP) -> None:
-        
-        self.role = role
-        self.competencies = competencies
-        self.capabilities = capabilities
-        self.tone = tone
-        self.lang = lang
-        self.extra_instructions = extra_instructions
-        self.openai_api_key = openai_api_key
-        self.model = model
-        self.temperature = temperature
-
-    def general_answer(self, question: str, context: str=None):
-
-        task = """Given the above CONTEXT, your task is to answer the following question: """
-
-        response = openai_answer(role=self.role,
-                                 competencies=self.competencies,
-                                 capabilities=self.capabilities,
-                                 task=task,
-                                 question=question,
-                                 context=context,
-                                 lang=self.lang,
-                                 tone=self.tone,
-                                 extra_instructions=self.extra_instructions,
-                                 openai_api_key=self.openai_api_key,
-                                 model=self.model)
+
+from .utils import *
+from .config import *
+
+class Agent:
+
+    def __init__(self, role= '', 
+                 competencies='', 
+                 capabilities= '',
+                 tone= '',
+                 lang= 'same',
+                 extra_instructions= '',
+                 openai_api_key: str=AGENTS_OPENAI_API_KEY, 
+                 model: str=AGENTS_MODEL,
+                 temperature: float=AGENTS_MODEL_TEMP) -> None:
+        
+        self.role = role
+        self.competencies = competencies
+        self.capabilities = capabilities
+        self.tone = tone
+        self.lang = lang
+        self.extra_instructions = extra_instructions
+        self.openai_api_key = openai_api_key
+        self.model = model
+        self.temperature = temperature
+
+    def general_answer(self, question: str, context: str=None):
+
+        task = """Given the above CONTEXT, your task is to answer the following question: """
+
+        response = openai_answer(role=self.role,
+                                 competencies=self.competencies,
+                                 capabilities=self.capabilities,
+                                 task=task,
+                                 question=question,
+                                 context=context,
+                                 lang=self.lang,
+                                 tone=self.tone,
+                                 extra_instructions=self.extra_instructions,
+                                 openai_api_key=self.openai_api_key,
+                                 model=self.model)
         return response
```

### Comparing `special_agents-1.0.6/src/special_agents/agents/ContentCreator.py` & `special_agents-1.0.7/src/special_agents/agents/ContentCreator.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,103 +1,103 @@
-from ..utils import *
-from ..Agent import Agent as BaseAgent
-
-class ContentCreator(BaseAgent):
-
-    def __init__(self, role= '', 
-                 competencies='', 
-                 capabilities= '',
-                 tone= '',
-                 lang= '',
-                 extra_instructions= '',
-                 openai_api_key: str=AGENTS_OPENAI_API_KEY, 
-                 model: str=AGENTS_MODEL,
-                 temperature: float=AGENTS_MODEL_TEMP) -> None:
-
-        super().__init__(role, 
-                 competencies, 
-                 capabilities,
-                 tone,
-                 lang,
-                 extra_instructions,
-                 openai_api_key, 
-                 model,
-                 temperature)
-        
-        self.role = 'Content Creator'
-        self.competencies = """
-        Expert in personal and business branding tactics
-        Outstanding copywriting, social media, or video production skills
-        Strong knowledge of SEO best practices
-        Significant experience creating high-quality marketing content
-        Capable of managing multiple competing priorities
-        Comprehensive understanding of impactful marketing tactics
-        Identify customers’ needs and recommend new topics
-
-        """
-        self.capabilities = """
-        
-        Create and publish engaging content for various platforms such as website, social media, blog, etc.
-        Use SEO best practices to drive traffic to digital channels
-        Collaborate across teams to determine and solve campaign objectives
-        Monitor digital engagement metrics
-        Promote offerings to reach new audiences
-        Research market trends and developments relevant to campaign subject matter
-
-        """
-
-    def general_answer(self, question: str, context: str=None):
-        return super().general_answer(question=question, context=context)
-
-    def write_linkedin_post(self, context: str): 
-
-        task = """Considering your competencies and utilizing your capabilities, given the above CONTEXT, your task is to write a social media post that suits LinkedIn."""
-        question = """Write a compelling LinkedIn post rich in details that considers the best practices and promotes users to engage and interact for the post to go viral for the audience most relevant to the CONTEXT."""
-
-        response = openai_answer(role=self.role,
-                                 competencies=self.competencies,
-                                 capabilities=self.capabilities,
-                                 task=task,
-                                 question=question,
-                                 context=context,
-                                 lang=self.lang,
-                                 tone=self.tone,
-                                 extra_instructions=self.extra_instructions,
-                                 openai_api_key=self.openai_api_key,
-                                 model=self.model)
-        return response
-    
-    def write_facebook_post(self, context: str): 
-
-        task = """Considering your competencies and utilizing your capabilities, given the above CONTEXT, your task is to write a social media post that suits Facebook."""
-        question = """Write a compelling rich in details Facebook post that considers the best practices and promotes users to engage and interact for the post to go viral for the audience most relevant to the CONTEXT."""
-
-        response = openai_answer(role=self.role,
-                                 competencies=self.competencies,
-                                 capabilities=self.capabilities,
-                                 task=task,
-                                 question=question,
-                                 context=context,
-                                 lang=self.lang,
-                                 tone=self.tone,
-                                 extra_instructions=self.extra_instructions,
-                                 openai_api_key=self.openai_api_key,
-                                 model=self.model)
-        return response
-    
-    def write_blog_article(self, context: str): 
-
-        task = """Considering your competencies and utilizing your capabilities, given the above CONTEXT, your task is to write a blog article."""
-        question = """Write a compelling long blog article rich in details that considers the best SEO practices using the appropriate keywords for the audience most relevant to the CONTEXT."""
-
-        response = openai_answer(role=self.role,
-                                 competencies=self.competencies,
-                                 capabilities=self.capabilities,
-                                 task=task,
-                                 question=question,
-                                 context=context,
-                                 lang=self.lang,
-                                 tone=self.tone,
-                                 extra_instructions=self.extra_instructions,
-                                 openai_api_key=self.openai_api_key,
-                                 model=self.model)
+from ..utils import *
+from ..Agent import Agent as BaseAgent
+
+class ContentCreator(BaseAgent):
+
+    def __init__(self, role= '', 
+                 competencies='', 
+                 capabilities= '',
+                 tone= '',
+                 lang= '',
+                 extra_instructions= '',
+                 openai_api_key: str=AGENTS_OPENAI_API_KEY, 
+                 model: str=AGENTS_MODEL,
+                 temperature: float=AGENTS_MODEL_TEMP) -> None:
+
+        super().__init__(role, 
+                 competencies, 
+                 capabilities,
+                 tone,
+                 lang,
+                 extra_instructions,
+                 openai_api_key, 
+                 model,
+                 temperature)
+        
+        self.role = 'Content Creator'
+        self.competencies = """
+        Expert in personal and business branding tactics
+        Outstanding copywriting, social media, or video production skills
+        Strong knowledge of SEO best practices
+        Significant experience creating high-quality marketing content
+        Capable of managing multiple competing priorities
+        Comprehensive understanding of impactful marketing tactics
+        Identify customers’ needs and recommend new topics
+
+        """
+        self.capabilities = """
+        
+        Create and publish engaging content for various platforms such as website, social media, blog, etc.
+        Use SEO best practices to drive traffic to digital channels
+        Collaborate across teams to determine and solve campaign objectives
+        Monitor digital engagement metrics
+        Promote offerings to reach new audiences
+        Research market trends and developments relevant to campaign subject matter
+
+        """
+
+    def general_answer(self, question: str, context: str=None):
+        return super().general_answer(question=question, context=context)
+
+    def write_linkedin_post(self, context: str): 
+
+        task = """Considering your competencies and utilizing your capabilities, given the above CONTEXT, your task is to write a social media post that suits LinkedIn."""
+        question = """Write a compelling LinkedIn post rich in details that considers the best practices and promotes users to engage and interact for the post to go viral for the audience most relevant to the CONTEXT."""
+
+        response = openai_answer(role=self.role,
+                                 competencies=self.competencies,
+                                 capabilities=self.capabilities,
+                                 task=task,
+                                 question=question,
+                                 context=context,
+                                 lang=self.lang,
+                                 tone=self.tone,
+                                 extra_instructions=self.extra_instructions,
+                                 openai_api_key=self.openai_api_key,
+                                 model=self.model)
+        return response
+    
+    def write_facebook_post(self, context: str): 
+
+        task = """Considering your competencies and utilizing your capabilities, given the above CONTEXT, your task is to write a social media post that suits Facebook."""
+        question = """Write a compelling rich in details Facebook post that considers the best practices and promotes users to engage and interact for the post to go viral for the audience most relevant to the CONTEXT."""
+
+        response = openai_answer(role=self.role,
+                                 competencies=self.competencies,
+                                 capabilities=self.capabilities,
+                                 task=task,
+                                 question=question,
+                                 context=context,
+                                 lang=self.lang,
+                                 tone=self.tone,
+                                 extra_instructions=self.extra_instructions,
+                                 openai_api_key=self.openai_api_key,
+                                 model=self.model)
+        return response
+    
+    def write_blog_article(self, context: str): 
+
+        task = """Considering your competencies and utilizing your capabilities, given the above CONTEXT, your task is to write a blog article."""
+        question = """Write a compelling long blog article rich in details that considers the best SEO practices using the appropriate keywords for the audience most relevant to the CONTEXT."""
+
+        response = openai_answer(role=self.role,
+                                 competencies=self.competencies,
+                                 capabilities=self.capabilities,
+                                 task=task,
+                                 question=question,
+                                 context=context,
+                                 lang=self.lang,
+                                 tone=self.tone,
+                                 extra_instructions=self.extra_instructions,
+                                 openai_api_key=self.openai_api_key,
+                                 model=self.model)
         return response
```

### Comparing `special_agents-1.0.6/src/special_agents/agents/FullStackDeveloper.py` & `special_agents-1.0.7/src/special_agents/agents/FullStackDeveloper.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,73 +1,73 @@
-from ..utils import *
-from ..Agent import Agent as BaseAgent
-
-class FullStackDeveloper(BaseAgent):
-
-    def __init__(self, role= '', 
-                 competencies='', 
-                 capabilities= '',
-                 tone= '',
-                 lang= '',
-                 extra_instructions= '',
-                 openai_api_key: str=AGENTS_OPENAI_API_KEY, 
-                 model: str=AGENTS_MODEL,
-                 temperature: float=AGENTS_MODEL_TEMP) -> None:
-
-        super().__init__(role, 
-                 competencies, 
-                 capabilities,
-                 tone,
-                 lang,
-                 extra_instructions,
-                 openai_api_key, 
-                 model,
-                 temperature)
-        
-        self.role = 'Full Stack Software Engineer'
-        self.competencies = """
-        - Bachelor’s degree with a concentration in Computer Science, Computer Engineering or related subject
-        - 5+ years of experience in Back-end engineering.
-        - 5+ years of experience in developing highly interactive web applications.
-        - Strong knowledge and first-hand experience frontend and backend stacks, languages and frameworks.
-        - Strong knowledge and first-hand experience in web applications; modular and reusable.
-        - Experience in Microservices architecture, RabbitMQ, Node.js, Redis, Memcache or Varnish.
-        - Knowledge in Object-Oriented Design Patterns.
-        - Knowledge in Enterprise Integration Patterns.
-        - Strong communication skills and ability to work in a dynamic environment.
-        """
-        self.capabilities = """
-        - Build robust and scalable software applications, APIs, services and middle-ware components as well as modifications of existing software.
-        - Design and create services and define system architecture for your projects, and contribute and provide feedback to other team members.
-        - Enhance code quality through writing unit tests, automation and performing code reviews.
-        - Brainstorm for ideas to technologies, platform and products and see your ideas grow and flourish.
-        - Work with the product and design teams to understand end-user requirements, formulate use cases, and then translate that into a pragmatic and effective technical solution.
-        - Solve challenging technical problems and successfully deliver results on schedule.
-        - Developing new and maintaining existing user-facing features
-        - Write client-side and server-side code for web-based applications, create fast, easy-to-use, high volume production applications.
-        - Ensuring the technical feasibility of UI/UX designs.
-        - Contribute to presentation layer standards and practices.
-        - Contribute to testing and implementation approach for presentation layer.
-        - Prototype future interfaces.
-        - Collaborating closely with the product team and other team members and stakeholders .
-        """
-
-    def general_answer(self, question: str, context: str=None):
-        return super().general_answer(question=question, context=context)
-
-    def write_code_documentation(self, context: str): 
-
-        task = """Considering your competencies and utilizing your capabilities, given the above CONTEXT, your task is to write the necessary code documentation"""
-        question = """Add the necessary docstrings in google style and the important inline comments to the code presented in the CONTEXT WITHOUT changing the code itself"""
-
-        response = openai_answer(role=self.role,
-                                 competencies=self.competencies,
-                                 capabilities=self.capabilities,
-                                 task=task,
-                                 question=question,
-                                 context=context,
-                                 lang=self.lang,
-                                 tone=self.tone,
-                                 extra_instructions=self.extra_instructions,
-                                 openai_api_key=self.openai_api_key,
-                                 model=self.model)
+from ..utils import *
+from ..Agent import Agent as BaseAgent
+
+class FullStackDeveloper(BaseAgent):
+
+    def __init__(self, role= '', 
+                 competencies='', 
+                 capabilities= '',
+                 tone= '',
+                 lang= '',
+                 extra_instructions= '',
+                 openai_api_key: str=AGENTS_OPENAI_API_KEY, 
+                 model: str=AGENTS_MODEL,
+                 temperature: float=AGENTS_MODEL_TEMP) -> None:
+
+        super().__init__(role, 
+                 competencies, 
+                 capabilities,
+                 tone,
+                 lang,
+                 extra_instructions,
+                 openai_api_key, 
+                 model,
+                 temperature)
+        
+        self.role = 'Full Stack Software Engineer'
+        self.competencies = """
+        - Bachelor’s degree with a concentration in Computer Science, Computer Engineering or related subject
+        - 5+ years of experience in Back-end engineering.
+        - 5+ years of experience in developing highly interactive web applications.
+        - Strong knowledge and first-hand experience frontend and backend stacks, languages and frameworks.
+        - Strong knowledge and first-hand experience in web applications; modular and reusable.
+        - Experience in Microservices architecture, RabbitMQ, Node.js, Redis, Memcache or Varnish.
+        - Knowledge in Object-Oriented Design Patterns.
+        - Knowledge in Enterprise Integration Patterns.
+        - Strong communication skills and ability to work in a dynamic environment.
+        """
+        self.capabilities = """
+        - Build robust and scalable software applications, APIs, services and middle-ware components as well as modifications of existing software.
+        - Design and create services and define system architecture for your projects, and contribute and provide feedback to other team members.
+        - Enhance code quality through writing unit tests, automation and performing code reviews.
+        - Brainstorm for ideas to technologies, platform and products and see your ideas grow and flourish.
+        - Work with the product and design teams to understand end-user requirements, formulate use cases, and then translate that into a pragmatic and effective technical solution.
+        - Solve challenging technical problems and successfully deliver results on schedule.
+        - Developing new and maintaining existing user-facing features
+        - Write client-side and server-side code for web-based applications, create fast, easy-to-use, high volume production applications.
+        - Ensuring the technical feasibility of UI/UX designs.
+        - Contribute to presentation layer standards and practices.
+        - Contribute to testing and implementation approach for presentation layer.
+        - Prototype future interfaces.
+        - Collaborating closely with the product team and other team members and stakeholders .
+        """
+
+    def general_answer(self, question: str, context: str=None):
+        return super().general_answer(question=question, context=context)
+
+    def write_code_documentation(self, context: str): 
+
+        task = """Considering your competencies and utilizing your capabilities, given the above CONTEXT, your task is to write the necessary code documentation"""
+        question = """Add the necessary docstrings in google style and the important inline comments to the code presented in the CONTEXT WITHOUT changing the code itself"""
+
+        response = openai_answer(role=self.role,
+                                 competencies=self.competencies,
+                                 capabilities=self.capabilities,
+                                 task=task,
+                                 question=question,
+                                 context=context,
+                                 lang=self.lang,
+                                 tone=self.tone,
+                                 extra_instructions=self.extra_instructions,
+                                 openai_api_key=self.openai_api_key,
+                                 model=self.model)
         return response
```

### Comparing `special_agents-1.0.6/src/special_agents/agents/ProductManager.py` & `special_agents-1.0.7/src/special_agents/agents/ProductManager.py`

 * *Ordering differences only*

 * *Files 17% similar despite different names*

```diff
@@ -1,126 +1,126 @@
-from ..utils import *
-from ..Agent import Agent as BaseAgent
-
-class ProductManager(BaseAgent):
-
-    def __init__(self, role= '', 
-                 competencies='', 
-                 capabilities= '',
-                 tone= '',
-                 lang= '',
-                 extra_instructions= '',
-                 openai_api_key: str=AGENTS_OPENAI_API_KEY, 
-                 model: str=AGENTS_MODEL,
-                 temperature: float=AGENTS_MODEL_TEMP) -> None:
-
-        super().__init__(role, 
-                 competencies, 
-                 capabilities,
-                 tone,
-                 lang,
-                 extra_instructions,
-                 openai_api_key, 
-                 model,
-                 temperature)
-        
-        self.role = 'Product Manager'
-        self.competencies = """
-        -BS in Computer Science or equivalent industry experience
-        -2+ years of product management or related industry experience
-        -1+ years of experience working on a B2B SaaS product
-        -High level of understanding of web development practices
-        -Strong understanding of digital analytics and conversion rate optimization processes
-        -Strong ability to refine and priorities product backlog in fast-moving environment
-        -Strong understanding of the Digital ecosystem, website design, content types, mobile and tablet applications, web technologies and digital marketing best practices.
-        -Proficient at writing user stories and defining acceptance criteria
-        -Experience going through a full product lifecycle, integrating customer feedback into product requirements.
-        -Excellent analytical skills, with the ability to interrogate project metrics to identify areas for continuous improvement
-        -Excellent written and verbal communication skills with business and technicalstakeholders at all levels
-        """
-        self.capabilities = """
-        -Owning the product vision and key objectives ensuring this aligns to the overall Business goals.
-        -Delivering and maintaining the roadmap and product strategy
-        -Producing product performance reports
-        -Partnering with UX team to build delightful features with solid designs
-        -Transforming ideas and feedback into a product vision and roadmap
-        -Understanding with customer problems in order to collect user needs, requirements, and pain points
-        -Utilizing performance metrics and data analysis to refine and improve product impact
-        -Working closely with the Technical team to execute and deliver roadmap milestones.
-        -Understand, communicate and drive optimization of all leading metrics and KPIs 
-        """
-
-    def general_answer(self, question: str, context: str=None):
-        return super().general_answer(question=question, context=context)
-
-
-    def write_user_story(self, context: str):
-        """
-        Write the best user story based on the given context.
-
-        Args:
-            context (str): The context for writing the user story.
-
-        Returns:
-            str: The detailed user story including acceptance criteria.
-        """
-
-        # Define the task and question for the user story
-        task = """Considering your competencies and utilizing your capabilities, given the above CONTEXT, your task is to write the best user story."""
-        question = """Write the detailed user story including its acceptance criteria in the following format:
-        Background: [one sentence]
-        Scenario: [the user story]
-        Acceptance Criteria: [bullet points]"""
-
-        # Call the openai_answer function to generate the user story
-        response = openai_answer(role=self.role,
-                                competencies=self.competencies,
-                                capabilities=self.capabilities,
-                                task=task,
-                                question=question,
-                                context=context,
-                                lang=self.lang,
-                                tone=self.tone,
-                                extra_instructions=self.extra_instructions,
-                                openai_api_key=self.openai_api_key,
-                                model=self.model)
-        return response
-    
-    def write_release_notes(self, context: str):
-        """
-        Write the release notes based on the given context.
-
-        Args:
-            context (str): The context for writing the release notes.
-
-        Returns:
-            str: The detailed release notes.
-        """
-
-        # Define the task and question for the release notes
-        task = """Considering your competencies and utilizing your capabilities, given the above CONTEXT, your task is to write the release notes."""
-        question = """Write the detailed release notes including its acceptance criteria in the following format:
-        Overview
-        [brief overview in less than 5 sentences]
-        
-        New Features 
-        [review of the new features in bullet points]
-        
-        Features Enhancements
-        [review of the enhancements in bullet points]
-        
-        Fixed Issues
-        [review of the bug fixes and fixed issues in bullet points]"""
-
-        # Call the openai_answer function to generate the user story
-        response = openai_answer(role=self.role,
-                                competencies=self.competencies,
-                                capabilities=self.capabilities,
-                                task=task,
-                                question=question,
-                                context=context,
-                                lang=self.lang,
-                                tone=self.tone,
-                                extra_instructions=self.extra_instructions,
-                                openai_api_key=self.openai_api_key,
-                                model=self.model)
+from ..utils import *
+from ..Agent import Agent as BaseAgent
+
+class ProductManager(BaseAgent):
+
+    def __init__(self, role= '', 
+                 competencies='', 
+                 capabilities= '',
+                 tone= '',
+                 lang= '',
+                 extra_instructions= '',
+                 openai_api_key: str=AGENTS_OPENAI_API_KEY, 
+                 model: str=AGENTS_MODEL,
+                 temperature: float=AGENTS_MODEL_TEMP) -> None:
+
+        super().__init__(role, 
+                 competencies, 
+                 capabilities,
+                 tone,
+                 lang,
+                 extra_instructions,
+                 openai_api_key, 
+                 model,
+                 temperature)
+        
+        self.role = 'Product Manager'
+        self.competencies = """
+        -BS in Computer Science or equivalent industry experience
+        -2+ years of product management or related industry experience
+        -1+ years of experience working on a B2B SaaS product
+        -High level of understanding of web development practices
+        -Strong understanding of digital analytics and conversion rate optimization processes
+        -Strong ability to refine and priorities product backlog in fast-moving environment
+        -Strong understanding of the Digital ecosystem, website design, content types, mobile and tablet applications, web technologies and digital marketing best practices.
+        -Proficient at writing user stories and defining acceptance criteria
+        -Experience going through a full product lifecycle, integrating customer feedback into product requirements.
+        -Excellent analytical skills, with the ability to interrogate project metrics to identify areas for continuous improvement
+        -Excellent written and verbal communication skills with business and technicalstakeholders at all levels
+        """
+        self.capabilities = """
+        -Owning the product vision and key objectives ensuring this aligns to the overall Business goals.
+        -Delivering and maintaining the roadmap and product strategy
+        -Producing product performance reports
+        -Partnering with UX team to build delightful features with solid designs
+        -Transforming ideas and feedback into a product vision and roadmap
+        -Understanding with customer problems in order to collect user needs, requirements, and pain points
+        -Utilizing performance metrics and data analysis to refine and improve product impact
+        -Working closely with the Technical team to execute and deliver roadmap milestones.
+        -Understand, communicate and drive optimization of all leading metrics and KPIs 
+        """
+
+    def general_answer(self, question: str, context: str=None):
+        return super().general_answer(question=question, context=context)
+
+
+    def write_user_story(self, context: str):
+        """
+        Write the best user story based on the given context.
+
+        Args:
+            context (str): The context for writing the user story.
+
+        Returns:
+            str: The detailed user story including acceptance criteria.
+        """
+
+        # Define the task and question for the user story
+        task = """Considering your competencies and utilizing your capabilities, given the above CONTEXT, your task is to write the best user story."""
+        question = """Write the detailed user story including its acceptance criteria in the following format:
+        Background: [one sentence]
+        Scenario: [the user story]
+        Acceptance Criteria: [bullet points]"""
+
+        # Call the openai_answer function to generate the user story
+        response = openai_answer(role=self.role,
+                                competencies=self.competencies,
+                                capabilities=self.capabilities,
+                                task=task,
+                                question=question,
+                                context=context,
+                                lang=self.lang,
+                                tone=self.tone,
+                                extra_instructions=self.extra_instructions,
+                                openai_api_key=self.openai_api_key,
+                                model=self.model)
+        return response
+    
+    def write_release_notes(self, context: str):
+        """
+        Write the release notes based on the given context.
+
+        Args:
+            context (str): The context for writing the release notes.
+
+        Returns:
+            str: The detailed release notes.
+        """
+
+        # Define the task and question for the release notes
+        task = """Considering your competencies and utilizing your capabilities, given the above CONTEXT, your task is to write the release notes."""
+        question = """Write the detailed release notes including its acceptance criteria in the following format:
+        Overview
+        [brief overview in less than 5 sentences]
+        
+        New Features 
+        [review of the new features in bullet points]
+        
+        Features Enhancements
+        [review of the enhancements in bullet points]
+        
+        Fixed Issues
+        [review of the bug fixes and fixed issues in bullet points]"""
+
+        # Call the openai_answer function to generate the user story
+        response = openai_answer(role=self.role,
+                                competencies=self.competencies,
+                                capabilities=self.capabilities,
+                                task=task,
+                                question=question,
+                                context=context,
+                                lang=self.lang,
+                                tone=self.tone,
+                                extra_instructions=self.extra_instructions,
+                                openai_api_key=self.openai_api_key,
+                                model=self.model)
         return response
```

### Comparing `special_agents-1.0.6/src/special_agents/utils.py` & `special_agents-1.0.7/src/special_agents/utils.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,99 +1,99 @@
-from openai import OpenAI
-from .config import *
-
-def openai_answer(role, 
-                  competencies, 
-                  capabilities, 
-                  task, 
-                  question, 
-                  context=None, 
-                  lang='same', 
-                  tone='friendly', 
-                  temperature=AGENTS_MODEL_TEMP, 
-                  extra_instructions='', 
-                  openai_api_key=AGENTS_OPENAI_API_KEY, 
-                  model=AGENTS_MODEL):
-    
-
-    """
-    Generate a response from OpenAI's model based on specified user role, competencies, capabilities, and a given task.
-
-    This function configures a message to OpenAI's API portraying a specific user role, its competencies, and capabilities,
-    then asks a question related to a task in a specified language and tone. The response is influenced by additional instructions and temperature settings.
-
-    Args:
-        role (str): The role of the virtual assistant.
-        competencies (str): Describes what the assistant is competent to handle.
-        capabilities (str): Describes the functional capabilities of the assistant.
-        task (str): A specific task or the type of questions the assistant is expected to handle.
-        question (str): The actual question posed to the assistant.
-        context (str): Additional context to help the assistant understand the scenario.
-        lang (str): The language in which the assistant should respond.
-        tone (str): The desired tone of the response (e.g., formal, friendly).
-        temperature (float): Controls the randomness of the response. Higher values mean more random responses.
-        extra_instructions (str, optional): Additional instructions to fine-tune the assistant's response.
-        openai_api_key (str): The API key for OpenAI. Defaults to AGENTS_OPENAI_API_KEY.
-        model (str, optional): The model used to generate the response. Defaults to AGENTS_MODEL.
-
-    Returns:
-        str: The response from the OpenAI model as a text string.
-
-    Examples:
-        >>> response = openai_answer(
-                role="Technical Support",
-                competencies="Software troubleshooting and customer support",
-                capabilities="Answering technical queries, providing solutions",
-                task="Assist users in resolving software issues",
-                question="How do I fix a connection issue?",
-                context="The user is experiencing intermittent connection.",
-                lang="English",
-                tone="professional",
-                extra_instructions="Be concise and direct.",
-                temperature=0.5
-            )
-        >>> print(response)
-        "To fix a connection issue, you should first check if your internet service provider..."
-    """
-    
-    # TODO: 
-    # wrap in a back off function to handle OpenAIrate limits.
-    # add context and question compression function to not exceed max allowed tokens 
-    
-    try:
-        client=OpenAI(
-                api_key = openai_api_key
-            )
-            
-        if context:
-            system_content = f"""
-                ROLE: You are a {role}. 
-                Your competencies are: {competencies}. 
-                Your capabilities are: {capabilities}. 
-                CONTEXT: {context}.
-                TASK: {task}.
-                INSTRUCTIONS:
-                - Answer in the {lang} language.
-                - Make your answer in a {tone} tone.
-                {extra_instructions}"""
-        else:
-            system_content = f"""
-                ROLE: You are a {role}. 
-                Your competencies are: {competencies}. 
-                Your capabilities are: {capabilities}. 
-                TASK: {task}
-                INSTRUCTIONS:
-                - Answer in the {lang} language.
-                - Make your answer in a {tone} tone.
-                {extra_instructions}"""
-        
-        response = client.chat.completions.create(
-            model = model,
-            temperature = temperature,
-            messages = [
-                {"role": "system", "content": system_content},
-                {"role": "user", "content": question}
-            ]
-        )
-        return response.choices[0].message.content
-    except Exception as err:
+from openai import OpenAI
+from .config import *
+
+def openai_answer(role, 
+                  competencies, 
+                  capabilities, 
+                  task, 
+                  question, 
+                  context=None, 
+                  lang='same', 
+                  tone='friendly', 
+                  temperature=AGENTS_MODEL_TEMP, 
+                  extra_instructions='', 
+                  openai_api_key=AGENTS_OPENAI_API_KEY, 
+                  model=AGENTS_MODEL):
+    
+
+    """
+    Generate a response from OpenAI's model based on specified user role, competencies, capabilities, and a given task.
+
+    This function configures a message to OpenAI's API portraying a specific user role, its competencies, and capabilities,
+    then asks a question related to a task in a specified language and tone. The response is influenced by additional instructions and temperature settings.
+
+    Args:
+        role (str): The role of the virtual assistant.
+        competencies (str): Describes what the assistant is competent to handle.
+        capabilities (str): Describes the functional capabilities of the assistant.
+        task (str): A specific task or the type of questions the assistant is expected to handle.
+        question (str): The actual question posed to the assistant.
+        context (str): Additional context to help the assistant understand the scenario.
+        lang (str): The language in which the assistant should respond.
+        tone (str): The desired tone of the response (e.g., formal, friendly).
+        temperature (float): Controls the randomness of the response. Higher values mean more random responses.
+        extra_instructions (str, optional): Additional instructions to fine-tune the assistant's response.
+        openai_api_key (str): The API key for OpenAI. Defaults to AGENTS_OPENAI_API_KEY.
+        model (str, optional): The model used to generate the response. Defaults to AGENTS_MODEL.
+
+    Returns:
+        str: The response from the OpenAI model as a text string.
+
+    Examples:
+        >>> response = openai_answer(
+                role="Technical Support",
+                competencies="Software troubleshooting and customer support",
+                capabilities="Answering technical queries, providing solutions",
+                task="Assist users in resolving software issues",
+                question="How do I fix a connection issue?",
+                context="The user is experiencing intermittent connection.",
+                lang="English",
+                tone="professional",
+                extra_instructions="Be concise and direct.",
+                temperature=0.5
+            )
+        >>> print(response)
+        "To fix a connection issue, you should first check if your internet service provider..."
+    """
+    
+    # TODO: 
+    # wrap in a back off function to handle OpenAIrate limits.
+    # add context and question compression function to not exceed max allowed tokens 
+    
+    try:
+        client=OpenAI(
+                api_key = openai_api_key
+            )
+            
+        if context:
+            system_content = f"""
+                ROLE: You are a {role}. 
+                Your competencies are: {competencies}. 
+                Your capabilities are: {capabilities}. 
+                CONTEXT: {context}.
+                TASK: {task}.
+                INSTRUCTIONS:
+                - Answer in the {lang} language.
+                - Make your answer in a {tone} tone.
+                {extra_instructions}"""
+        else:
+            system_content = f"""
+                ROLE: You are a {role}. 
+                Your competencies are: {competencies}. 
+                Your capabilities are: {capabilities}. 
+                TASK: {task}
+                INSTRUCTIONS:
+                - Answer in the {lang} language.
+                - Make your answer in a {tone} tone.
+                {extra_instructions}"""
+        
+        response = client.chat.completions.create(
+            model = model,
+            temperature = temperature,
+            messages = [
+                {"role": "system", "content": system_content},
+                {"role": "user", "content": question}
+            ]
+        )
+        return response.choices[0].message.content
+    except Exception as err:
         return(f"Unexpected {err=}, {type(err)=}")
```

### Comparing `special_agents-1.0.6/src/special_agents.egg-info/SOURCES.txt` & `special_agents-1.0.7/src/special_agents.egg-info/SOURCES.txt`

 * *Files identical despite different names*

