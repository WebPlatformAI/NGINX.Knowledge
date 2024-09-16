# Solution:
https://serverfault.com/questions/416787/nginx-403-forbidden-error-hosting-in-user-home-directory
>Nginx needs to have read permission the files that should be served AND have execute permission in each of the parent directories along the path from the root to the served files.

```
sudo chmod a+x /home
sudo chmod a+x /home/$USER
chmod a+x $web_root
```
