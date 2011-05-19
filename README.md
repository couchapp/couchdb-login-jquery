# The least code way to add login to your CouchApp

If you write CouchApps using jQuery but don't want to use [Evently](http://github.com/couchapp/evently), this is what you want. It is the simplest way to add login to your app.

It weighs in at 70 lines of JS, or about 2kb minified.

## Usage

Simple Example usage:

     $("#mylogindiv").couchLogin()

This will turn #mylogindiv into an interactive form that lets the user signup and login with a minimum of fuss. If you have code you want to run, when they log in, you can provide callbacks.

Example Usage with optional `loggedIn` and `loggedOut` callbacks:

    $("#mylogindiv").couchLogin({
        loggedIn : function(userCtx) {
            alert("hello "+userCtx.name);
        }, 
        loggedOut : function() {
            alert("bye bye");
        }
    });

   
# Other

Join other CouchApp devs http://groups.google.com/group/couchapp

Copyright Chris Anderson 2011

Apache 2.0 License
