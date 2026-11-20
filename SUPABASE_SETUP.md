# Configuración de reservas en Supabase

1. Crea un proyecto en [Supabase](https://supabase.com/).
2. En **SQL Editor**, ejecuta el contenido de `supabase-setup.sql`.
3. En **Project Settings → API**, copia el Project URL y la clave pública `anon`/publishable en `supabase-config.js`. No uses nunca la `service_role` key en la web.
4. En **Authentication → Providers**, habilita Email. Deshabilita el registro público y crea desde **Authentication → Users** el usuario del administrador.
5. Publica los archivos del sitio en un hosting HTTPS. Abre `admin.html` e inicia sesión con el usuario creado.

El panel requiere iniciar sesión. La clave pública del navegador solo puede crear reservas y consultar fecha/horas ocupadas; las políticas RLS reservan la lectura de datos personales y la actualización de estados para usuarios autenticados.
