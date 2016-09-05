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
中介層用來處理請求中的參數  
網址列的參數應該讓路由器來處理  
laravel會自行使用加密  
在表單上要加一個隱藏的"_token"input  

不要再把檔案名字打錯了啦!!!

