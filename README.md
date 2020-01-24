# phpInit
Aprendendo PHP com Laravel

#Installing Laravel
  - Utilizando o Composer para gerenciar as dependências e utilizar o laravel para construir o projeto
  - https://getcomposer.org/
  - baixar o laravel com o comando 'composer composer global require laravel/installer'
# Via Composer Create-Project
  - composer create-project --prefer-dist laravel/laravel Projeto
  
# Rodando o projeto
  - tem que está na pasta do projeto criado, assim executar o comando 'php artisan serve'
   
# phpInit
Aprendendo PHP com Laravel

#Installing Laravel
  - Utilizando o Composer para gerenciar as dependências e utilizar o laravel para construir o projeto
  - https://getcomposer.org/
  - baixar o laravel com o comando 'composer composer global require laravel/installer'
# Via Composer Create-Project
  - composer create-project --prefer-dist laravel/laravel Projeto
  
# Rodando o projeto
  - tem que está na pasta do projeto criado, assim executar o comando 'php artisan serve'
   
+--------+----------------------------------------+------------------------+------------------+------------------------------------------------------------------------+--------------+
| Domain | Method                                 | URI                    | Name             | Action                                                                 | Middleware   |
+--------+----------------------------------------+------------------------+------------------+------------------------------------------------------------------------+--------------+
|        | GET|HEAD                               | /                      |                  | Closure                                                                | web          |
|        | GET|HEAD                               | api/user               |                  | Closure                                                                | api,auth:api |
|        | GET|HEAD                               | app                    | app              | Closure                                                                | web          |
|        | GET|HEAD                               | app/profile            | app.profile      | Closure                                                                | web          |
|        | GET|HEAD                               | app/user               | app.user         | Closure                                                                | web          |
|        | GET|HEAD                               | comregras/{nome}/{n}   |                  | Closure                                                                | web          |
|        | GET|HEAD                               | home                   | home             | App\Http\Controllers\HomeController@index                              | web,auth     |
|        | POST                                   | login                  |                  | App\Http\Controllers\Auth\LoginController@login                        | web,guest    |
|        | GET|HEAD                               | login                  | login            | App\Http\Controllers\Auth\LoginController@showLoginForm                | web,guest    |
|        | POST                                   | logout                 | logout           | App\Http\Controllers\Auth\LoginController@logout                       | web          |
|        | GET|HEAD                               | ola/{nome}/{sobrenome} |                  | Closure                                                                | web          |
|        | POST                                   | password/email         | password.email   | App\Http\Controllers\Auth\ForgotPasswordController@sendResetLinkEmail  | web,guest    |
|        | POST                                   | password/reset         | password.update  | App\Http\Controllers\Auth\ResetPasswordController@reset                | web,guest    |
|        | GET|HEAD                               | password/reset         | password.request | App\Http\Controllers\Auth\ForgotPasswordController@showLinkRequestForm | web,guest    |
|        | GET|HEAD                               | password/reset/{token} | password.reset   | App\Http\Controllers\Auth\ResetPasswordController@showResetForm        | web,guest    |
|        | GET|HEAD                               | produtos               | meusprodutos     | Closure                                                                | web          |
|        | POST                                   | register               |                  | App\Http\Controllers\Auth\RegisterController@register                  | web,guest    |
|        | GET|HEAD                               | register               | register         | App\Http\Controllers\Auth\RegisterController@showRegistrationForm      | web,guest    |
|        | PUT                                    | requisicoes            |                  | Closure                                                                | web          |
|        | GET|HEAD                               | requisicoes            |                  | Closure                                                                | web          |
|        | OPTIONS                                | requisicoes            |                  | Closure                                                                | web          |
|        | PATCH                                  | requisicoes            |                  | Closure                                                                | web          |
|        | DELETE                                 | requisicoes            |                  | Closure                                                                | web          |
|        | POST                                   | requisicoes            |                  | Closure                                                                | web          |
|        | GET|HEAD                               | seunome/{nome?}        |                  | Closure                                                                | web          |
|        | GET|HEAD                               | teste                  |                  | Closure                                                                | web          |
|        | GET|HEAD|POST|PUT|PATCH|DELETE|OPTIONS | todosprodutos1         |                  | Illuminate\Routing\RedirectController                                  | web          |
|        | GET|HEAD                               | todosprodutos2         |                  | Closure                                                                | web          |
+--------+----------------------------------------+------------------------+------------------+------------------------------------------------------------------------+--------------+

