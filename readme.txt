Práctica 9 DCA - Sistema de Control de Versiones

Creación de alias globales de Git:
git config --global alias.co checkout
git config --global alias.br branch
git config --global alias.st status

Creación de alias locales de Git:
git config alias.pushall 'push --all origin'

Uso de git bisect:
1. Iniciar bisect: git bisect start
2. Marcar commit actual como malo: git bisect bad
3. Marcar commit inicial como bueno: git bisect good <commit-inicial>
4. Git irá mostrando commits intermedios
5. Probar cada versión y marcar como good/bad
6. Al encontrar el commit problemático: git bisect reset
