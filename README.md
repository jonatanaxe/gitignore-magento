# gitignore magento e wordpress


# Config-Wordpress
Voce pode editar esse adicionar esse codigo no seu wp-config.php apos a linha 
define('WP_DEBUG', false);
Pode editar o código dependendo da necessidade do projeto

# Recomendados na aplicação
Por padrão, eles são gerados aleatoriamente para você. 
Mas o WordPress na verdade tem uma ferramenta gratuita que você pode usar para  gerar novas chaves aleatórias.
https://api.wordpress.org/secret-key/1.1/salt/

# Recomendados no servidor

## Apache
```
<files wp-config.php>
order allow,deny
deny from all
</files>
```
## Nginx

```
location ~* wp-config.php { deny all; }
```

