### Git y GitHub Commands Cheat Sheet

#### **1. Configuración Inicial**

1. **Configurar tu Nombre y Correo Electrónico:**
   ```bash
   git config --global user.name "Tu Nombre"
   git config --global user.email "tuemail@example.com"
   ```

2. **Inicializar un Nuevo Repositorio:**
   ```bash
   git init
   ```

#### **2. Creación y Gestión de Repositorios**

1. **Crear un Nuevo Repositorio en GitHub:**
   - Navega a GitHub y crea un nuevo repositorio.
   - Copia la URL del repositorio.

2. **Clonar un Repositorio Existente:**
   ```bash
   git clone https://github.com/tu-usuario/tu-repositorio.git
   ```

3. **Agregar un Repositorio Remoto:**
   ```bash
   git remote add origin https://github.com/tu-usuario/tu-repositorio.git
   ```

4. **Verificar Repositorios Remotos:**
   ```bash
   git remote -v
   ```

#### **3. Trabajar con Archivos y Commits**

1. **Agregar Archivos al Staging Area:**
   ```bash
   git add .
   ```

2. **Hacer un Commit de los Cambios:**
   ```bash
   git commit -m "Mensaje del commit"
   ```

3. **Ver el Estado del Repositorio:**
   ```bash
   git status
   ```

4. **Ver el Historial de Commits:**
   ```bash
   git log
   ```

#### **4. Trabajo con Ramas**

1. **Crear una Nueva Rama:**
   ```bash
   git branch nombre-de-rama
   ```

2. **Cambiar a una Rama:**
   ```bash
   git checkout nombre-de-rama
   ```

3. **Crear y Cambiar a una Nueva Rama:**
   ```bash
   git checkout -b nombre-de-rama
   ```

4. **Eliminar una Rama:**
   ```bash
   git branch -d nombre-de-rama
   ```

#### **5. Sincronización con Repositorios Remotos**

1. **Enviar Cambios a un Repositorio Remoto:**
   ```bash
   git push origin nombre-de-rama
   ```

2. **Obtener Cambios desde un Repositorio Remoto:**
   ```bash
   git pull origin nombre-de-rama
   ```

3. **Traer (fetch) Cambios desde un Repositorio Remoto:**
   ```bash
   git fetch origin
   ```

#### **6. Fusión y Resolución de Conflictos**

1. **Fusionar una Rama en la Rama Actual:**
   ```bash
   git merge nombre-de-rama
   ```

2. **Resolver Conflictos de Fusión:**
   - Abre los archivos en conflicto y resuelve los conflictos manualmente.
   - Después de resolver los conflictos, agrega los archivos al staging area:
     ```bash
     git add archivo-resuelto
     ```
   - Completa la fusión:
     ```bash
     git commit
     ```

#### **7. Otras Operaciones Útiles**

1. **Revertir un Commit:**
   ```bash
   git revert id-del-commit
   ```

2. **Restablecer el Repositorio a un Commit Anterior:**
   ```bash
   git reset --hard id-del-commit
   ```

3. **Guardar Cambios en Stash:**
   ```bash
   git stash
   ```

4. **Aplicar Cambios desde Stash:**
   ```bash
   git stash apply
   ```

#### **8. Integración Continua y Despliegue**

1. **Configurar CI/CD en GitHub Actions:**
   - Crea un archivo de workflow en `.github/workflows`.
   - Define los pasos necesarios para la integración y despliegue continuo en el archivo de configuración YAML.