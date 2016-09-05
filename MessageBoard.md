#MessageBoard
##Controller
*   Account  

      >postLogin  
      >getLogout  
      >postRegister  

*   User  

      >getShowPersonalFile  
      >postEditPersonalFile  
      >postChangePWD  
      >postEditFriends  
      
##Model


//laravel中如果在routes.php裡面使用Route::controller('params', 'controllerNames');  
就不能使用這樣的形態Route::get('params', ['middleware' => 'middlewareName','uses' => 'ControllerName']);
Route::controller('params', 'controllerNames');  
雖然可以減少路由器的工作，但是維護和使用就比較不容易懂
需要預先處理的函數也沒辦法先處理，會直接轉到controller，除非都用不到model不然可能還是用一般方法會比較好

