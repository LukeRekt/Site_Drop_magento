# Loja Magento Da Rapaziada

Esse repositório foi criado para armazenar as versões da loja da rapaziada

### TODO

* Mudar o layoult da loja com logo e nome novo.
* adicionar os produtos escolhidos pela equipe.
* mudar o template básico do sistema de emails
* Futuro:Fazer sistema autómatico de checagem de produtos

### OBS
* o arquivo Anatocaoes site.txt na raiz do rep possui algumas infos sobre a montagem dos site indev que devem ser desfeitas ao dar deploy para o host.
o arquivo Index.php tem a seguinte condição adicionada: 

`if(!file_exists(__DIR__ . '/app/etc/env.php')){
     $installerPath = "http://$_SERVER[HTTP_HOST]$_SERVER[REQUEST_URI]installer.php";
     header("Location: $installerPath");
 } else`