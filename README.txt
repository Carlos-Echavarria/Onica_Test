El Playbook fue probado en el entorno de lab al que tenía acceso que fue un CentOS 7.5.1804, se debe :

1) Contar con ansible instalado
2) Descomprimir el zip, en el mismo hay un archivo de inventario, el playbook y este readme
3) El mismo pide que se pasen 3 variables al momento de ejecutarlo, primero la contraseña a configurar de root para mysql, luego el usuario con privilegios de sudo local y finalmente la contraseña de ese usuario : 

ansible-playbook -i inventario_toolbox_ve -K toolbox_ve_playbook.yml --extra-vars “mysql_root_password=PASS1 ansible_user=USERID ansible_password=PASS2”