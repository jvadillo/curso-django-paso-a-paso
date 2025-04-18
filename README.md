# Curso de iniciación a Django paso a paso

Este es un curso diseñado para aprender desarrollar aplicaciones web con **Django desde cero**. Siguiendo la metodología *Learn by doing* está pensado para que vayas aprendiendo los fundamentos básicos de Django mientras construyes tu primera aplicación web.

## Conocimientos previos

El curso requiere unos conocimientos básicos de **Python, HTML y CSS**.
Del mismo modo partirá de la base de que tienes **Python y PIP** instalados en el sistema.

Puedes encontrar cursos y tutoriales sobre HTML, CSS y Python en [www.jonvadillo.com](http://jonvadillo.com)

Si no dispones de conocimientos previos en Python o te gustaría consolidarlos, tienes un disponible el libro gratuito "Apende Python desde cero a experto" en [este enlace](https://leanpub.com/aprende-python) (también puedes acceder directamente al repositorio [desde aquí](https://github.com/jvadillo/aprende-python-desde-cero-a-experto)).


## Material

En este repositorio puedes encontrar todas las presentaciones para ir aprendiendo Django desde cero y paso a paso. Por otro lado en esta misma página también puedes encontrar una guía resumen con todos los pasos necesarios para crear una aplicación web con Django.
### Slides

1.  Introducción y fundamentos básicos: [slides](https://github.com/jvadillo/curso-django-paso-a-paso/blob/master/slides/01-Django-Introduccion.pdf)
2.  Crea tu primer proyecto en Django: [slides](https://github.com/jvadillo/curso-django-paso-a-paso/blob/master/slides/02-Django-Crear%20proyecto.pdf)
3.  Crea tu primera aplicación en django: [slides](https://github.com/jvadillo/curso-django-paso-a-paso/blob/master/slides/03-Django-Creacion%20de%20una%20aplicacion.pdf)
4.  El modelo en Django,  acceso a datos y la aplicación de administrador ([slides](https://github.com/jvadillo/curso-django-paso-a-paso/blob/master/slides/04-Django-%20Bases%20de%20datos,%20modelo%20y%20aplicacion%20de%20administrador.pdf))
5.  Vistas y plantillas en Django ([slides](https://github.com/jvadillo/curso-django-paso-a-paso/blob/master/slides/05-Django-Vistas%20y%20plantillas.pdf))
6.  Vistas basadas en clases ([slides](https://github.com/jvadillo/curso-django-paso-a-paso/blob/master/slides/06-Django-Vistas%20basadas%20en%20clases.pdf))
7. Formularios en Django ([slides](https://github.com/jvadillo/curso-django-paso-a-paso/blob/master/slides/07-Django-Formularios.pdf))

### Video-tutoriales
#### Curso Django
- Curso Django - Paso 1. Introducción + Instalación URL ([ir al video](https://youtu.be/yZDH6vH3iM8))
- Curso Django - Paso 2. Crear un proyecto URL ([ir al video](https://youtu.be/cIXG5GkoTOE))
- Curso Django - Paso 3. Crear una aplicación URL ([ir al video](https://youtu.be/Ewe4QAP0wuU))
- Curso Django - Paso 4. Crear una vista URL ([ir al video](https://youtu.be/nYe-h06cEvM))
- Curso Django - Paso 5. Modelos y acceso a datos URL ([ir al video](https://youtu.be/Br_Z-8BF9Qg))
- Curso Django - Paso 6. Aplicación de administración URL ([ir al video](https://youtu.be/9yDd8OrIVfk))
- Curso Django - Paso 7. Creación de vistas Básicas URL ([ir al video](https://youtu.be/E_8fAfGvKVs))
- Curso Django - Paso 8. Plantillas (templates) URL ([ir al video](https://youtu.be/th3VMi-a8mk))
- Curso Django - Paso 9. Herencia de plantillas URL ([ir al video](https://youtu.be/zcBPKBq6v84))
- Django paso a paso. Paso 10: archivos estáticos (CSS, JS, ...) URL ([ir al video](https://youtu.be/yP8HeZ6Hdlw))
- Django paso a paso. Paso 11: acceso a URLs mediante el nombre ([ir al video](https://youtu.be/cIvfIbU_3z0))
- Django paso a paso. Paso 12: Vistas genéricas basadas en clases (DetailView y ListView) URL ([ir al video](https://youtu.be/4dGG5G9Ixsc))
- Django paso a paso. Paso 13: Formularios (1/3) URL ([ir al video](https://youtu.be/zsE3JwM63wU))
- Django paso a paso. Paso 14 Formularios (2/3) ([ir al video](https://youtu.be/KFVW3-a5k4c))

#### Otros
- Tutorial Python: cómo utilizar entornos virtuales (virtualenv y configuración en PyCharm y VS Code) ([ir al video](https://youtu.be/lJrs7P9eKXc))

- Videotutorial: Crear un API con Django ([ir al video](https://youtu.be/XqRBb_4CLS4))


## Hands on!

Tan solo necesitas seguir  los pasos descritos en esta sección para lograr desarrollar tu primera aplicación web con Django. 
Recuerda que como pre-requisito tienes que tener **Python y PIP** instalado en el sistema. ¡Happy Coding!

### PASO 1: Instala Django

#### Entorno virtual

Para el desarrollo en local de proyectos con Python **es recomendable aislar las dependencias de nuestros proyectos mediante entornos virtuales**. Este es un paso opcional, por lo que si acabas de iniciarte en Python puedes saltártelo y una vez tengas algo más de soltura podrás pasar al manejo de entornos virtuales.

Si te decides por utilizar entornos virtuales, el primer paso será crear uno y así disponer de un entorno aislado donde instalar nuestras dependencias (por ejemplo, Django) sin que nos afecten otras que tengamos instaladas en nuestro sistema. Para crear el entorno virtual en Windows, abre el CMD y ejecuta:
    
      python -m venv nombre_del_entorno

 Activar el entorno (se activa automáticamente al crearlo)
    
      nombre_del_entorno\Scripts\activate
    
    
Podemos saber si estamos dentro de un entorno virtual porque la consola nos pondrá en toto momento el nombre del entorno en el que nos encontramos entre paréntesis. En este caso:


	(nombre_del_entorno) C:\Users\developer>

Recuerda que podemos saber las dependencias que tenemos instaladas en un entorno virtual ejecutando el comando `pip freeze`. Si lo hacemos ahora, no mostrará nada ya que acabamos de crear el entorno.

#### Instalación de Django

Recuerda que en este curso asumimos que tienes [Python](https://www.python.org/downloads/) y el gestor de paquetes [PIP](https://pip.pypa.io/en/latest/installation/) instalado en tu sistema. Para instalar Django ejecuta el siguiente comando:

- Windows: `py -m pip install Django`
- Linux/MAC: `python -m pip install Django`

Si ejecutas el comando `py -m pip freeze` una vez instalado Django, verás cómo muestra varias dependecias que ha instalado (aparecerá Django y otras dependencias que Django necesita):

	(.env) C:\Users\developer>pip freeze
	asgiref==3.8.1
	Django==5.1.7
	sqlparse==0.5.3
	tzdata==2025.2

Si en lugar de utilizar `venv` quieres utilizar virtualenvwapper pero tienes dudas respecto a su instalación y configuración en PyCharm o Visual Studio Code, [puedes ver este video](https://youtu.be/lJrs7P9eKXc) donde se explica todo lo que necesitas saber.

#### Diferencia entre `python` y `py`

En Windows puedes utilizar tanto `python` como `py`. La diferencia está en que para utilizar `python` necesitas haber añadido a la variable de entorno `PATH` la versión de Python que quieres utilizar. Por el contrario, `py` es un launcher instalado normalmente en `C:\Windows` que permite indicar la versión de Python a utilizar (por defecto utilizará la más actual que encuentre instalada en el sistema).


### PASO 2: Crea tu primer proyecto

Crea el proyecto Django llamado `empresaDjango`:

      django-admin startproject empresaDjango
    
En caso de que el anterior comando te dé error en Windows, utiliza el comando alternativo: 

	py -m django startproject empresaDjango

o el comando:

	python -m django startproject empresaDjango

La estructura de ficheros resultante es la siguiente:
    
    ```
     empresaDjango/
         manage.py
         project/
     	__init__.py
     	settings.py
     	urls.py
     	wsgi.py
    
    ```
    
Como puedes ver, empresaDjango será el paquete que incluirá todo nuestro proyecto. Entra dentro de la carpeta del proyecto (`cd empresaDjango`) y ahora inicia el servidor con el comando `py manage.py runserver`.
Puedes comprobar que puedes acceder correctamente abriendo desde el navegador la página que te indica: http://127.0.0.1:8000/

Para cerrar el servidor pulsa las teclas CTRL+C.

### PASO 3: Crea tu primera aplicación

Estando dentro del directorio del proyecto, crea la aplicación llamada `appEmpresaDjango` ejecutando el siguiente comando:

`py manage.py startapp appEmpresaDjango`

En caso de que tengas algún problema para ejecutarlo, prueba con el siguiente comando:

`py -m django startapp appEmpresaDjango`

La estructura de ficheros resultante será la siguiente:

```
 project/
     manage.py
     project/
 	__init__.py
 	settings.py
 	urls.py
 	wsgi.py
     app/
 	migrations/
 	    __init__.py
 	__init__.py
 	admin.py
 	apps.py
 	models.py
 	tests.py
 	urls.py
 	views.py

```

Incluir a aplicación dentro del fichero `settings.py` del proyecto, añadiendo el nombre a la lista `INSTALLED_APPS`:
	
	 INSTALLED_APPS = [
	 	'appEmpresaDjango',
	 	# ...
	 ]

### PASO 4: Crea una nueva vista y configura su ruta de acceso

Dentro del directorio de la app, abrir `views.py` y añadir lo siguiente:

```python
from django.http import HttpResponse

def index(request):
    return HttpResponse("Listado de departamentos")
```
    
Cada aplicación de Django necesitará un archivo `urls.py` para redirigir cada URL a la que intenta acceder el usuario con la función correspondiente de `views.py`. Crea el archivo `urls.py` dentro de la carpeta de la aplicación y añade el patrón para la siguiente ruta:
   ```python
from django.urls import path
from . import views
   
urlpatterns = [
    path('', views.index, name='index'),
]
   ```
Con esto le estaremos diciendo que la función `index()` recién creada será la encargada de responder a las llamadas a esa ruta (en este caso la ruta será '/').

Como Django nos permite tener múltiples aplicaciones dentro de un proyecto, vamos a decirle qué ruta seguirán las llamadas a la aplicación `appEmpresaDjango`. Para ello, dentro del directorio del proyecto hay que editar el archivo `urls.py` e incluir la redirección al fichero `urls.py` de la aplicación `appEmpresaDjango`. El resultado debe ser el siguiente (no olvides importar la librería `include` de `django.urls`):

   ```python
from django.contrib import admin
from django.urls import include, path
  
urlpatterns = [
    path('appEmpresaDjango/', include('appEmpresaDjango.urls')),
    path('admin/', admin.site.urls),
]
   ```

En resumen, la idea es que cada aplicación gestiones sus rutas con su propio `urls.py`, pero también tenemos que decirle al proyecto qué URLs gestionará cada aplicación (mediante su propio `urls.py`). En el ejemplo anterior, todas las rutas que vayan a `/appEmpresaDjango` se gestionarán desde el urls.py que hemos creado en la aplicación.

Para comprobar que la vista funciona perfectamente, prueba a iniciar el servidor y acceder a la ruta: http://127.0.0.1:8000/appEmpresaDjango/

### PASO 5: Crea el modelo de nuestra aplicación

Para consultar y manipular datos en la base de datos utilizaremos los modelos. Los modelos son clases de Python que le permiten a Django crear el esquema de base de datos con todas sus tablas y acceder a los objetos almacenados en ella.  Edita el fichero `models.py` de la aplicación creando las clases Departamento, Habilidad y Empleado:

```python
from django.db import models
 
class Departamento(models.Model):
    # No es necesario crear un campo para la Primary Key, Django creará automáticamente un IntegerField.
    nombre = models.CharField(max_length=50)
    telefono = models.IntegerField()

class Habilidad(models.Model):
    # No es necesario crear un campo para la Primary Key, Django creará automáticamente un IntegerField.
    nombre = models.CharField(max_length=50)
 
class Empleado(models.Model):
    # Campo para la relación one-to-many (un empleado pertenece a un departamento)
    departamento = models.ForeignKey(Departamento, on_delete=models.CASCADE)
    # Campo para la relación many-to-many (un empleado tiene varias habilidades)
    habilidades = models.ManyToManyField(Habilidad)
    nombre = models.CharField(max_length=40)
    fecha_nacimiento = models.DateField()
    # Es posible indicar un valor por defecto mediante 'default'
    antiguedad = models.IntegerField(default=0)
    # Para permitir propiedades con valor null, añadiremos las opciones null=True, blank=True.       	
```

Aplica los cambios realizados en el modelo mediante los siguientes comandos:
    
```
python manage.py makemigrations appEmpresaDjango
python manage.py migrate
```

#### Añade y consulta registros desde la API de Django

Accede al intérprete interactivo de Django escribiendo el siguiente comando:

	python manage.py shell

Una vez dentro, ya puedes comenzar a crear y consultar registros.
   ```python
	>>> from appEmpresaDjango.models import Departamento, Habilidad, Empleado
	>>> departamento = Departamento(nombre="Oficina Tecnica", telefono="945010101")
	>>> departamento.save()
	# Django le asigna un id.
	>>> departamento.id
	1
	
	# Acceder a sus atributos
	>>> departamento.nombre
	'Oficina Tecnica'
	
	>>> Departamento.objects.all()
	<QuerySet [<Departamento: Departamento object (1)>]>
	
	>>> Departamento.objects.filter(nombre__contains='Oficina').count()
	1
	
	# Mostrar los empleados de un departamento.
	>>> departamento.empleado_set.all()
	<QuerySet []>
	
	# Crear un empleado, indicando el departamento.
	>>> empleado = Empleado(departamento=departamento, nombre="Markel Ugalde", fecha_nacimiento='1988-06-12', antiguedad="12")
	>>> departamento.save()
	
	
	# Opción alternativa para crear empleados a partir del departamento:
	>>> departamento.empleado_set.create(nombre='Mikel Uriarte', fecha_nacimiento='1985-01-23')
	<Empleado: Empleado object (1)>
	
	>>>> departamento.empleado_set.create(nombre='Ane Labastida', fecha_nacimiento='1987-12-14')
	<Empleado: Empleado object (2)>
	
	empleado = departamento.empleado_set.create(nombre='Luken Abarra', fecha_nacimiento='1989-05-12')
	
	# Es posible acceder desde el hijo a su padre.
	>>> empleado.departamento
	<Departamento: Departamento object (1)>
	
	>>> empleado.departamento.nombre
	'Oficina Tecnica'
	
	# Podemos conseguir un empleado por su primary key:
	empleado = Empleado.objects.get(pk=1)
	
	# También es posible acceder desde el padre a todos sus hijos.
	>>> departamento.empleado_set.all()
	<QuerySet [<Empleado: Empleado object (1)>, <Empleado: Empleado object (2)>, <Empleado: Empleado object (3)>]>
	
	>>>> departamento.empleado_set.count()
	3
	
	>>>> quit()
   ```

Es recomendable incluir un método ```__str__()``` dentro de cada clase de nuestro modelo para que sea invocado al llamar a los métodos *print* o *str* de nuestros objetos, que por ejemplo son usados internamente desde los formularios de la aplicación de administración que ofrece Django por defecto. De esta forma tendremos la posibilidad de mostrar objetos binarios como texto e identificarlos más fácilmente.

```python
def __str__(self):
        return self.nombre
```

### PASO 6: Utiliza la aplicación de Administración de Django para visualizar y añadir registros

La aplicación de administración permite visualizar la información de nuestros modelos de forma sencilla. Crear un usuario "adminDjango" (contraseña: "adminDjango") para la aplicación de administración:
    
```
     python manage.py createsuperuser
    
```
    
Editar el fichero `admin.py` para registrar las clases de nuestro modelo y que se puedan ver en la aplicación de administración por defecto que trae Django:
    
```
from django.contrib import admin
from .models import Departamento, Habilidad, Empleado
admin.site.register(Departamento)
admin.site.register(Habilidad)
admin.site.register(Empleado)
```

Iniciar el servidor y entrar
    
```
py manage.py runserver
```
    
Entrar en la aplicación [http://127.0.0.1:8000/admin](http://127.0.0.1:8000/admin) y añadir algunas entradas en cada entidad para tener un juego de ensayo que luego se pueda ver desde la aplicación [http://127.0.0.1:8000/appEmpresaDjango](http://127.0.0.1:8000/appEmpresaDjango)

### PASO 7: Crea las vistas y urls para interactuar con el modelo

Creamos las vistas correspondientes a las siguientes URLs:

| URL | Descripción de la vista |
| -- | -- |
| /appEmpresaDjango  | Muestra todos los departamentos  |
| /appEmpresaDjango/departamentos/<:id>  | Muestra los detalles de un departamento a partir del ID indicado  |
| /appEmpresaDjango/departamentos/<:id>/empleados  | Muestra los empleados del departamento con el ID indicado  |
| /appEmpresaDjango/empleados/<:id>  | Muestra los detalles del empleado con el ID indicado  |
| /appEmpresaDjango/habilidades/<:id>  | Muestra los detalles de la habilidad con el ID indicado  |

Creamos las vistas (cada vista estará definida por una función):
```python
from django.http import HttpResponse
from .models import Departamento, Habilidad, Empleado


#devuelve el listado de departamentos
def index_departamentos(request):
	departamentos = Departamento.objects.order_by('nombre')
	output = ', '.join([d.nombre for d in departamentos])
	return HttpResponse(output)

#devuelve los datos de un departamento
def show_departamento(request, departamento_id):
	departamento = Departamento.objects.get(pk=departamento_id)
	output = f'Detalles del departamento: {departamento.id}, {departamento.nombre}, {departamento.telefono}'
	return HttpResponse(output)

#devuelve los empleados de un departamento
def index_empleados(request, departamento_id):
	departamento = Departamento.objects.get(pk=departamento_id)
	output = ', '.join([e.nombre for e in departamento.empleado_set.all()])
	return HttpResponse(output)

#devuelve los detalles de un empleado
def show_empleado(request, empleado_id):
	empleado = Empleado.objects.get(pk=empleado_id)
	output = f'Detalles del empleado: {empleado.id}, {empleado.nombre}, {empleado.fecha_nacimiento}, {empleado.antiguedad}, {str(empleado.departamento)}. Habilidades: {[h.nombre for h in empleado.habilidades.all()]}'
	return HttpResponse(output)

#devuelve los detalles de una habilidad
def show_habilidad(request, habilidad_id):
	habilidad = Habilidad.objects.get(pk=habilidad_id)
	output = f'Detalles de la habilidad: {habilidad.id}, {habilidad.nombre}. Empleados: {[e.nombre for e in habilidad.empleado_set.all()]}'
	return HttpResponse(output)
```

Creamos las URLs que redirijan las peticiones a las vistas creadas:
```python
from django.urls import path
from . import views

urlpatterns = [
    path('', views.index_departamentos, name='index'),
    path('departamentos/<int:departamento_id>/', views.show_departamento, name='detail'),
    path('departamentos/<int:departamento_id>/empleados', views.index_empleados, name='empleados'),
    path('empleados/<int:empleado_id>', views.show_empleado, name='empleado'),
    path('habilidades/<int:habilidad_id>', views.show_habilidad, name='habilidad'),
]
```

Cuando hacemos referencia por ejemplo a `views.index`, está refiriéndose al método `index()` de `views.py`.

#### Opcional: mejora las vistas controlando errores 404

Utiliza el método `get_object_or_404` para controlar los casos en los que el registro de la petición no exista:

```python
from django.http import HttpResponse, Http404
from django.shortcuts import get_object_or_404, get_list_or_404
from .models import Departamento, Habilidad, Empleado


#devuelve el listado de departamentos
def index_departamentos(request):
	departamentos = get_list_or_404(Departamento.objects.order_by('nombre'))
	output = ', '.join([d.nombre for d in departamentos])
	return HttpResponse(output)

#devuelve los datos de un departamento
def show_departamento(request, departamento_id):
    departamento = get_object_or_404(Departamento, pk=departamento_id)
    output = f'Detalles del departamento: {departamento.id}, {departamento.nombre}, {departamento.telefono}'
    return HttpResponse(output)

#devuelve los empleados de un departamento
def index_empleados(request, departamento_id):
	departamento = get_object_or_404(Departamento, pk=departamento_id)
	output = ', '.join([e.nombre for e in departamento.empleado_set.all()])
	return HttpResponse(output)

#devuelve los detalles de un empleado
def show_empleado(request, empleado_id):
	empleado = get_object_or_404(Empleado, pk=empleado_id)
	output = f'Detalles del empleado: {empleado.id}, {empleado.nombre}, {empleado.fecha_nacimiento}, {empleado.antiguedad}, {str(empleado.departamento)}. Habilidades: {[h.nombre for h in empleado.habilidades.all()]}'
	return HttpResponse(output)

#devuelve los detalles de una habilidad
def show_habilidad(request, habilidad_id):
	habilidad = get_object_or_404(Habilidad, pk=habilidad_id)
	output = f'Detalles de la habilidad: {habilidad.id}, {habilidad.nombre}. Empleados: {[e.nombre for e in habilidad.empleado_set.all()]}'
	return HttpResponse(output)
```


### PASO 8: Utiliza plantillas para mostrar la información

Actualiza las vistas creadas en `views.py`:

```python
from django.shortcuts import get_object_or_404, get_list_or_404
from django.shortcuts import render
from .models import Departamento, Habilidad, Empleado

#devuelve el listado de empresas
def index_departamentos(request):
	departamentos = get_list_or_404(Departamento.objects.order_by('nombre'))
	context = {'lista_departamentos': departamentos }
	return render(request, 'index.html', context)

#devuelve los datos de un departamento
def show_departamento(request, departamento_id):
	departamento = get_object_or_404(Departamento, pk=departamento_id)
	context = {'departamento': departamento }
	return render(request, 'detail.html', context)

#devuelve los empelados de un departamento
def index_empleados(request, departamento_id):
	departamento = get_object_or_404(Departamento, pk=departamento_id)
	empleados =  departamento.empleado_set.all()
	context = {'departamento': departamento, 'empleados' : empleados }
	return render(request, 'empleados.html', context)

#devuelve los detalles de un empleado
def show_empleado(request, empleado_id):
	empleado = get_object_or_404(Empleado, pk=empleado_id)
	habilidades =  empleado.habilidades.all()
	context = { 'empleado': empleado, 'habilidades' : habilidades }
	return render(request, 'empleado.html', context)

# Devuelve los detalles de una habilidad
def show_habilidad(request, habilidad_id):
    habilidad = get_object_or_404(Habilidad, pk=habilidad_id)
    empleados =  habilidad.empleado_set.all()
    context = { 'empleados': empleados, 'habilidad' : habilidad }
    return render(request, 'habilidad.html', context)
```

Crea las plantillas (en una carpeta "templates" dentro del directorio de la aplicación) que definan la estructura de las páginas HTML resultantes:

Plantilla index.html:

```python
<!DOCTYPE html>
<html lang="en">
    <head>
        <link rel="stylesheet" href="style.css">
        <title>Listado de departamentos</title>
    </head>
    <body>
        <div id="content">
	     <h1>Gestor de Empleados</h1>
         <h2>Listado de departamentos</h2>
         {% if lista_departamentos %}
             <ul>
             {% for d in lista_departamentos %}
                 <li>
                     <a href="/appEmpresaDjango/departamentos/{{ d.id }}">{{ d.nombre}}</a>
                 </li>
             {% endfor %}
             </ul>
         {% else %}
         <p>No hay departamentos creados.</p>
         {% endif %}
        </div>
    </body>
</html>
```
Plantilla detail.html:

```python
<!DOCTYPE html>
<html lang="en">

<head>
    <link rel="stylesheet" href="style.css">
    <title>Detalle del departamento</title>
</head>

<body>
    <div id="content">
        <h1>Gestor de Empleados</h1>
        <h2>Datos del departamento</h2>
        {% if departamento %}
            <ul>
                <li>
                    {{ departamento.nombre}}
                </li>
                <li>
                    {{ departamento.telefono}}
                </li>
                <li>
                    <a href="/appEmpresaDjango/departamentos/{{ departamento.id }}/empleados">Ver empleados</a>
                </li>
            </ul>
        {% else %}
            <p>No existe este departamento.</p>
        {% endif %}
    </div>
</body>

</html>
```

Plantilla empleados.html:

```python
<!DOCTYPE html>
<html lang="en">

<head>
    <link rel="stylesheet" href="style.css">
    <title>Empleados del departamento</title>
</head>

<body>
    <div id="content">
        <h1>Gestor de Empleados</h1>
        <h2>Lista de empleados</h2>
        <h3>{{ departamento.nombre }}</h3>
        {% if empleados %}
            <ul>
                {% for e in empleados %}
                <li>
                    <a href="/appEmpresaDjango/empleados/{{ e.id }}">{{ e.nombre}}</a>
                </li>
                {% endfor %}
            </ul>
        {% else %}
            <p>No hay empleados creados.</p>
        {% endif %}
    </div>
</body>

</html>
```

Plantilla empleado.html:

```python
<!DOCTYPE html>
<html lang="en">

<head>
    <link rel="stylesheet" href="style.css">
    <title>Detalles del empleado</title>
</head>

<body>
    <div id="content">
        <h1>Gestor de Empleados</h1>
        <h2>Datos del empleado</h2>

        {% if empleado %}
            <ul>
                <li>
                    {{ empleado.nombre}}
                </li>
                <li>
                    {{ empleado.fecha_nacimiento}}
                </li>
                <li>
                    {{ empleado.antiguedad}}
                </li>
                <li>
                    <a href="/appEmpresaDjango/departamentos/{{ empleado.departamento.id }}">{{ empleado.departamento}}</a>
                </li>
            </ul>
            <h3>Lista de habilidades</h3>
            {% if habilidades %}
                <ol>
                    {% for h in habilidades %}
                        <li>
                            <a href="/appEmpresaDjango/habilidades/{{ h.id }}">{{ h.nombre}}</a>
                        </li>
                    {% endfor %}
                </ol>
            {% else %}
                <p>No tiene habilidades asociadas.</p>
            {% endif %}
        {% else %}
            <p>No existe este empleado.</p>
        {% endif %}
    </div>
</body>

</html>
```

Plantilla habilidad.html:

```python
<!DOCTYPE html>
<html lang="en">

<head>
    <link rel="stylesheet" href="style.css">
    <title>Detalles de la habilidad</title>
</head>

<body>
    <div id="content">
        <h1>Gestor de Empleados</h1>

        <h2>Datos de la habilidad</h2>

        {% if habilidad %}
            <h3>{{ habilidad.nombre}}</h3>
            <h3>Lista de empleados</h3>
            
            {% if empleados %}
            <ol>
                {% for e in empleados %}
                    <li>
                        <a href="/appEmpresaDjango/empleados/{{ e.id }}">{{ e.nombre}}</a>
                    </li>
                {% endfor %}
            </ol>
            {% else %}
                <p>No tiene empleados asociados.</p>
            {% endif %}
        {% else %}
            <p>No existe esta habilidad.</p>
        {% endif %}

    </div>
</body>

</html>
```


### PASO 9: La herencia en plantillas

Como puedes ver en las plantillas anteriores, hay mucho código HTML que se repite en todas las páginas creadas (cabecera, footer, etc). Además, ¿qué ocurriría si queremos cambiar la etiqueta <title> de nuestras páginas? Tendríamos que hacer el cambio en todos los ficheros, lo cual no es nada cómodo y puede dar lugar a errores. Para evitar esto, Django permite crear una plantilla base que contenga el “esqueleto” con todos los elementos comunes y definir bloques que puedan ser sobreescritos por las plantillas que la hereden. 

Crea una plantilla "base.html" que contenga toda la estructura común:
```html
<!DOCTYPE html>
<html lang="en">
    <head>
        <link rel="stylesheet" href="style.css">
        <title>{% block titulo %}Gestor de Empleados{% endblock %}</title>
    </head>
    <body>
        <div id="content">
	     <h1>Gestor de Empleados</h1>
            {% block contenido %}{% endblock %}
        </div>
    </body>
</html>
```


Las plantillas específicas que heredan de la plantilla base, deberán llevar una única directiva "extends" para indicar que van a heredar automáticamente el código de la plantilla base:

```python
#index.html:
{% extends "base.html" %}
```
Ahora cada plantilla simplemente tendrá que definir el contenido que quiere incluir dentro de los bloques indicados en la plantilla base (los que están definidos con las directivas `{% block %}` y `{% endblock %}`:
	
Plantilla index.html:

```python
{% extends "base.html" %}

{% block titulo %}Listado de departamentos{% endblock %}

{% block contenido %}
<h2>Listado de departamentos</h2>
{% if lista_departamentos %}
	<ul>
	{% for d in lista_departamentos %}
		<li>
		    <a href="/appEmpresaDjango/departamentos/{{ d.id }}">{{ d.nombre}}</a>
		</li>
	{% endfor %}
	</ul>
{% else %}
<p>No hay departamentos creados.</p>
{% endif %}
{% endblock %}
```
Plantilla detail.html:

```python
{% extends "base.html" %}

{% block titulo %} Detalle del departamento {% endblock %}

{% block contenido %}
<h2>Datos del departamento</h2>

{% if departamento %}
    <ul>
        <li>
            {{ departamento.nombre}}
        </li>
        <li>
            {{ departamento.telefono}}
        </li>
        <li>
            <a href="/appEmpresaDjango/departamentos/{{ departamento.id }}/empleados">Ver empleados</a>
        </li>
    </ul>
{% else %}
    <p>No existe este departamento.</p>
{% endif %}

{% endblock %}
```

Plantilla empleados.html:

```python
{% extends "base.html" %}

{% block titulo %} Empleados del departamento {% endblock %}

{% block contenido %}
<h2>Lista de empleados</h2>
<h3>{{ departamento.nombre }}</h3>
{% if empleados %}
	<ul>
	{% for e in empleados %}
		<li>
		    <a href="/appEmpresaDjango/empleados/{{ e.id }}">{{ e.nombre}}</a>
		</li>
	{% endfor %}
	</ul>
{% else %}
<p>No hay empleados creados.</p>
{% endif %}
{% endblock %}
```

Plantilla empleado.html:

```python
{% extends "base.html" %}

{% block titulo %} Detalles del empleado {% endblock %}

{% block contenido %}

<h2>Datos del empleado</h2>

{% if empleado %}
    <ul>
        <li>
            {{ empleado.nombre}}
        </li>
        <li>
            {{ empleado.fecha_nacimiento}}
        </li>
        <li>
            {{ empleado.antiguedad}}
        </li>
        <li>
            <a href="/appEmpresaDjango/departamentos/{{ empleado.departamento.id }}">{{ empleado.departamento}}</a>
        </li>
    </ul>
	<h3>Lista de habilidades</h3>
	{% if habilidades %}
		<ol>
		{% for h in habilidades %}
			<li><a href="/appEmpresaDjango/habilidades/{{ h.id }}">{{ h.nombre}}</a></li>
		{% endfor %}
		</ol>
	{% else %}
		<p>No tiene habilidades asociadas.</p>
	{% endif %}
{% else %}
    <p>No existe este empleado.</p>
{% endif %}

{% endblock %}
```

Plantilla habilidad.html:

```python
{% extends "base.html" %}

{% block titulo %} Detalles de la habilidad {% endblock %}

{% block contenido %}

<h2>Datos de la habilidad</h2>

{% if habilidad %}
    <h3>{{ habilidad.nombre}}</h3>
	<h3>Lista de empleados</h3>
	{% if empleados %}
		<ol>
		{% for e in empleados %}
			<li><a href="/appEmpresaDjango/empleados/{{ e.id }}">{{ e.nombre}}</a></li>
		{% endfor %}
		</ol>
	{% else %}
		<p>No tiene empleados asociados.</p>
	{% endif %}
{% else %}
    <p>No existe esta habilidad.</p>
{% endif %}

{% endblock %}
```
	
#### Opcional: Actualizar las URLs

En lugar de utilizar la ruta de la URL, podemos utilizar el nombre que le hemos dado en el mapeo definido en `urls.py`

Antes:
```html
<li><a href="/appEmpresaDjango/departamento/{{ d.id }}">{{ d.nombre }}</a></li>
```
Ahora
```html
<li><a href="{% url 'detail' d.id %}">{{ d.nombre}}</a></li>
```
Cambia también el resto de URLs en las vistas correspondientes.

Entrar en la aplicación [http://127.0.0.1:8000/appEmpresaDjango/](http://127.0.0.1:8000/appEmpresaDjango/)

### PASO 10: Incluir archivos estáticos	
	
Incluir archivos estáticos (CSS, imágenes, etc.) es muy sencillo en Django. Sigue los siguientes pasos para incluir un archivo .css llamado `estilos.css`:

En primer lugar crea un directorio llamado `static` dentro de la carpeta de tu aplicación. Será el directorio encargado de contener los archivos estáticos. Como en esta ocasión se trata de un archivo CSS, crearemos dentro una carpeta llamada CSS para así mantener nuestros ficheros organizados. Dentro crearemos un nuevo archivo llamado `estilos.css` con el siguiente contenido:
	
```css
h1 {
    color: blue;
}	
```
Nos servirá para comprobar que todo ha ido bien. A continuación, entra en el archivo `settings.py` de tu proyecto y añade la siguiente información para especificar dónde se ubican nuestros archivos estáticos:
	
```
STATICFILES_DIRS = [os.path.join(BASE_DIR, 'static')]
```
	
Hazlo justo debajo de `STATIC_URL = 'static/'`, es decir, como resultado quedará así:

```
STATIC_URL = 'static/'
STATICFILES_DIRS = [os.path.join(BASE_DIR, 'static')]
```
	
Ahora ya podremos incluir nuestro CSS en cualquier plantilla .html. Para ello debemos incluir en la primera línea la directiva `{% load static %}` y a la hora de referenciar el archivo CSS hacerlo de la siguiente forma:

```
<link rel="stylesheet" href="{% static 'css/estilos.css' %}">
```
	
## Contribuir
Toda contribución es más que bienvenida. Puedes contribuir con este libro de las siguientes:
- Ayuda a mejorar el material notificando errores, planteando mejoras o incluso nuevos ejercicios prácticos.
- Comparte y recomienda este libro o el repositorio en las redes sociales.
- Recuerda que puedes adquirir este libro por el precio que consideres (¡desde cero euros!)

Para contribuir puedes contactarme vía email a vadillo.jon@gmail.com

## Licencia

![Licencia_img](http://mirrors.creativecommons.org/presskit/buttons/80x15/png/by-nc-sa.png)

Este libro esta licenciado como [Creative Commons Attribution-NonCommercial-ShareAlike 4.0 International License](https://creativecommons.org/licenses/by-nc-sa/4.0/deed.es_ES) aunque no necesariamente las imágenes de su interior.

El código que contiene este [repositorio](https://github.com/jvadillo/aprende-python-desde-cero-a-experto/) se encuenta bajo la licencia [GNU GPL-3.0](https://github.com/jvadillo/aprende-python-desde-cero-a-experto/blob/master/LICENSE)
