# CWP User Used Quota, Custom CWP Module
Centos Web Panel Custom Module For Users Used Quota.
Module show used quota for User's home dir, mysql and emails

## How to install 
Edit this file (if the file doesn't exist, create it)

    /usr/local/cwpsrv/htdocs/resources/admin/include/3rdparty.php
    
add this line

    <li><a href="index.php?module=users_used_quota"><span class="icon16 icomoon-icon-arrow-right-3"></span>Users Used Quota</a></li>

    <script type="text/javascript">
        $(document).ready(function() {
                var newButtons = ''
                  +' <li>'
                  +' <a href="?module=users_used_quota" class=""><span aria-hidden="true" class="icon16 icomoon-icon-arrow-right-3"></span>Users Used Quota</a>'
                  +'</li>';
                $("ul#mn-15-sub").append(newButtons);
        });
    </script>

Download `users_used_quota.php`
Upload `users_used_quota.php` in `/usr/local/cwpsrv/htdocs/resources/admin/modules/`

You can access the module from `Plugins` Menu in CWP Menu

I am open to suggestion, feel free to pull request if you think you can improve my code.
