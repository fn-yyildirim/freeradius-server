
```bash
# install necessary dependencies, openldap-devel required for ldap auth support
dnf install openssl-devel openldap-devel

# append necessary parameters to add ldap auth support (not sure about --with-ldap but it works :D)
./configure --with-raddbdir=/etc/raddb --with-experimental-modules --with-ldap --with-libfreeradius-ldap-lib-dir=/usr/lib64 --with-libfreeradius-ldap-include-dir=/usr/include

make
sudo make install
```
