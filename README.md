# Ufocus
Aplicativo movil

Flujo de ramas
Nuestro equipo seguirá el flujo de trabajo GitFlow, el cual nos permitirá mantener una organización clara entre las ramas de desarrollo, nuevas funcionalidades y versiones en producción.

RAMAS PRINCIPALES
main: contiene siempre la última versión estable y lista para producción.
develop: rama base donde se integran las nuevas funcionalidades antes de pasar a producción.

RAMAS DE SOPORTE
feature/: usadas para desarrollar nuevas funcionalidades.
Se crean desde develop.
hotfix/: usadas para corregir errores críticos en main. Se crean desde main.
Ejemplo: hotfix/fix-auth-bug.
Al finalizar, se integran tanto a main como a develop.
release/: usadas para preparar una nueva versión estable.
Se crean desde develop.
Se realizan pruebas, documentación y ajustes.
Al finalizar, se fusionan en main y develop.

Flujo de trabajo
1. Crear rama feature/nueva-funcionalidad desde develop.
2. Desarrollar y probar localmente.
3. Abrir un Pull Request hacia develop.
4. El líder del equipo o un compañero revisa el PR (usando checklist).
5. Una vez aprobado, se hace merge en develop.
6. Cuando el proyecto esté listo para una entrega, se crea una rama release/x.x.x.
7. Después de pruebas finales, se fusiona en main y se etiqueta la versión.
8. Si aparece un bug urgente en producción, se crea un hotfix/.
