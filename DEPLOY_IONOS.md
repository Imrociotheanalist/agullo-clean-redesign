# Guia para Desplegar en IONOS

## Opcion 1: Descargar Archivos Compilados Directamente (MAS SIMPLE)

Ya tu web está publicada y compilada en Lovable:
**URL:** https://limpiezasagullo.lovable.app

Para subir a IONOS:

### Paso 1: Descargar la web publicada
1. Ve a: https://limpiezasagullo.lovable.app
2. 2. Usa una herramienta como `httrack` o descarga manualmente todos los archivos
   3. 3. O simplemente apunta tu dominio IONOS al subdominio de Lovable
     
      4. ### Paso 2: Subir a IONOS
      5. 1. Accede a tu panel de control de IONOS
         2. 2. Ve a la sección de "Archivo" o "FTP"
            3. 3. Sube los archivos descargados a la carpeta `public_html` o la raiz del dominio
               4. 4. Configura tu dominio en IONOS
                 
                  5. ---
                 
                  6. ## Opcion 2: Clonar desde GitHub y Compilar Localmente
                 
                  7. ### Requisitos:
                  8. - Node.js v16+ instalado
                     - - npm o yarn
                       - - Git instalado
                        
                         - ### Paso 1: Clonar el repositorio
                         - ```bash
                           git clone https://github.com/Imrociotheanalist/agullo-clean-redesign.git
                           cd agullo-clean-redesign
                           ```

                           ### Paso 2: Instalar dependencias
                           ```bash
                           npm install
                           # o
                           yarn install
                           ```

                           ### Paso 3: Compilar para produccion
                           ```bash
                           npm run build
                           # o
                           yarn build
                           ```

                           Esto generara una carpeta `/dist` con todos los archivos compilados listos para produccion.

                           ### Paso 4: Subir a IONOS
                           1. Accede a tu panel FTP de IONOS
                           2. 2. Sube todo el contenido de la carpeta `/dist` a `public_html` o raiz del dominio
                              3. 3. Asegurate que el archivo `index.html` este en la raiz
                                
                                 4. ---
                                
                                 5. ## Opcion 3: Apuntar DNS a Lovable (SIN COMPILAR)
                                
                                 6. Esta es la opcion mas rapida si quieres usar Lovable como hosting:
                                
                                 7. ### En IONOS:
                                 8. 1. Accede a tu gestor de dominios
                                    2. 2. Ve a "Configurar DNS"
                                       3. 3. Configura los registros DNS para apuntar a Lovable (contacta a Lovable para los valores exactos)
                                          4. 4. O crea un alias CNAME hacia limpiezasagullo.lovable.app
                                            
                                             5. ---
                                            
                                             6. ## Verificacion Final
                                             7. 1. Accede a tu dominio en IONOS
                                                2. 2. Verifica que todos los estilos y funciones funcionan correctamente
                                                   3. 3. Prueba todos los enlaces y secciones
                                                     
                                                      4. ## Problemas Comunes
                                                     
                                                      5. **Los estilos no cargan:**
                                                      6. - Verifica que los archivos CSS estén en la ubicación correcta
                                                         - - Revisa la consola del navegador (F12) para errores 404
                                                          
                                                           - **Las imagenes no aparecen:**
                                                           - - Asegurate que las rutas de las imagenes sean relativas
                                                             - - Verifica que las imagenes se subieron al mismo directorio
                                                              
                                                               - **Errores de JavaScript:**
                                                               - - Verifica que no hay rutas absolutas en el código
                                                                 - - Usa rutas relativas para todos los recursos
                                                                  
                                                                   - ---

                                                                   ## Contacto
                                                                   Email: rocioroman74@gmail.com
                                                                   Repositorio: https://github.com/Imrociotheanalist/agullo-clean-redesign
                                                                   Web en Lovable: https://limpiezasagullo.lovable.app
