### Laravel Commands Cheat Sheet

A continuación, se presentan los comandos organizados por prioridad:

#### **1. Instalación y Configuración del Proyecto**

1. **Instalar un Instalador Global para Laravel:**
   ```bash
   composer global require laravel/installer
   ```

2. **Crear un Proyecto con PHP y Laravel:**
   ```bash
   composer create-project --prefer-dist laravel/laravel proyecto-base
   ```

3. **Crear un Nuevo Proyecto usando el Instalador de Laravel:**
   ```bash
   laravel new project-name
   ```

#### **2. Configuración Posterior a la Clonación del Proyecto**

1. **Después de Clonar el Proyecto, Descargar Dependencias:**
   ```bash
   composer install
   ```

2. **Instalar Paquetería:**
   ```bash
   npm install
   ```

#### **3. Ejecución del Proyecto**

1. **Correr el Servidor (Back => PHP):**
   ```bash
   php artisan serve
   ```

2. **Correr el Proyecto con Todas sus Dependencias:**
   ```bash
   composer run
   ```

3. **Correr Front:**
   ```bash
   npm run dev
   ```

#### **4. Manejo de Migraciones**

1. **Si se Ejecuta pero Sale Error 500, lo Más Probable es que No Hayamos Hecho la Migración:**

2. **Migración Manual:**
   ```bash
   php artisan migrate
   ```

3. **Comando para Hacer una Migración Personalizada:**
   ```bash
   php artisan make:migration create_table-name_table
   ```

4. **Comando para Hacer una Migración Refrescando Todas las Tablas y sus Registros:**
   ```bash
   php artisan migrate:fresh
   ```

#### **5. Creación de Modelos y Seeders**

1. **Crear Nuevo Modelo:**
   ```bash
   php artisan make:model Product -mcr
   ```

2. **Este Comando Creará Todos los Seeders que Tengas:**
   ```bash
   php artisan db:seed --class=[nombreArchivo]
   ```

3. **Crear un Seeder:**
   ```bash
   php artisan make:seeder RolesTableSeeder
   ```

#### **6. Otros Comandos Útiles**

1. **Crear una Solicitud de Validación (Request):**
   ```bash
   php artisan make:request RoleRequest
   ```

2. **Instalar Ejecución de Pruebas de Código:**
   ```bash
   composer require --dev phpstan/phpstan
   ```

3. **Ejecutar Pruebas para Verificar Errores:**
   ```bash
   ./vendor/bin/phpstan analyse --level=0 app/
   ```

4. **Comando Autoload:**
   ```bash
   composer dump-autoload
   ```

5. **Limpiar Caché de Rutas:**
   ```bash
   php artisan route:clear
   ```

#### **7. Resolución de Problemas**

1. **Si No Funciona en Linux, Ejecutar:**
   ```bash
   /bin/bash -c "$(curl -fsSL https://php.new/install/linux)"
   ```
