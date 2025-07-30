# Developing AI Applications with Python and Flask  
## API Architectures  
![api_architectures](./static/08/api_architectures.png)  
## Tests  
![building_tests](./static/08/building_tests.png)  
## Module vs Package vs Library  
![module](./static/08/module.png)  
![package](./static/08/package.png)  
![package_init](./static/08/package_init.png)  
![library](./static/08/library.png)  
## Flask  
![config](./static/08/config.png)  
![app_structure](./static/08/app_structure.png)  
- Methods  
![methods](./static/08/methods.png)  
- Status  
![status](./static/08/status.png)  
- Request  
![extract_request_info](./static/08/extract_request_info.png)  
![response](./static/08/response.png)  
- Form  
![form](./static/08/form.png)  
- Dynamic Routing  
    ![dynamic_routing](./static/08/dynamic_routing.png)  
    ![dynamic_routing_specify_datatype](./static/08/dynamic_routing_specify_datatype.png)  
    - We can handle multiple routes with a single function by just stacking additional route decorators above the method which should be invoked when the route is called.  
    ```
    @app.route("/")
    @app.route("/home")
    @app.route("/index")
    def home():
        return "Hello World!"
    ```  
- Error Handler  
![error_handler](./static/08/error_handler.png)  
- Redirect & Dynamic URLs  
```
from flask import redirect

@app.route('/admin')
def admin():
    return redirect('/login')
```
```
from flask import url_for

@app.route('/admin')
def admin():
    return redirect(url_for('login'))

@app.route('/login')
def login():
    return "<Login Page>"
```  
# Python Decorator  
``` 
def jsonify_decorator(function):
    def modifyOutput():
        return {"output":function()}
    return modifyOutput

@jsonify_decorator
def hello():
    return 'hello world'

@jsonify_decorator
def add():
    num1 = input("Enter a number - ")
    num2 = input("Enter another number - ")
    return int(num1)+int(num2)
```  
