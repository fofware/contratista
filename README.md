# contratista
aplicación para gestionar proyectos

# Descripción de las tareas del contratista
La empresa recibe un requerimiento, este requerimento es evaluado y se genera un proyecto a partir de los items que lo conforman con materiales a comprar o servicios a subcontratar para poder cumplir con el requerimiento recibido.
A partir de este proyecto se solicita a los proveedores la cotización de productos y/o servicios (pudiendo solicitar cotización de un mismo item, servicio o material a distintos proveedores). Al tener todos los items valorizados, se conforma emite un presupuesto para ser presentado al cliente que hizo el requerimiento.
Este presupuesto puede tener modificaciones hasta terminar de acordar todos los items con el cliente antes de ser comfirmado y aceptado por el mismo.
Una vez aceptado el presupuesto, se debe informar a Facturación, cobranzas y pagos.
Facturación, Cobranzas y Pagos cada uno debe recibir la información pertinente para llevar a cabo sus funciones.
Facturación recibe el presupuesto con la información necesaria para facturar.
Cobranzas recibe la notificación de lo que fue facturado y cobra
Pagos recibe la información del presupuesto y los proveedores a los que debe emitir los pagos para dar comienzo a la obra.

Detalles más o menos estas etapas y procesos son los que se intentan automatizar para dar seguimiento a los proyectos que cada contratista gestiona.
# funciones
1. Requerimiento del Cliente
2. Generación de Proyecto: Un proyecto se conforma de items
   1. Materiales
      1. (Código)
      2. Descripción
         1. Proveedor
         2. Precio Unitario
         3. Cantidad
         4. Subtotal
         5. Estado
            1. Solicitado
            2. Presupuestado
            3. Aceptado
   2. Servicio
      1. Interno
         1. (Código)
         2. Descripción
         3. Departamento
         4. Costo
         5. Cantidad
         6. Subtotal
         7. Estado
            1. Solicitado
            2. Presupuestado
            3. Aceptado
      2. Externo
         1. (Código)
         2. Descripción
         1. Proveedor 
            1. Costo
            4. Cantidad
            5. Subtotal
            6. Estado
               1. Solicitado
               2. Presupuestado
               3. Aceptado
            7. Fecha
  3. Generación del Presupuesto para Cliente, al tener cada item del proyecto con un precio aceptado se confecciona el presupuesto para el cliente que queda en espera hasta su aceptación o rechazo, debiendo conservar un historial de modificaciones y/o consultas del cliente sobre el mismo y permitiendo ser madificado hasta ser aprobado o rechzado
     1. Estado
        1. Presentado
        2. Evaluación
        3. Negociando
        4. Aceptado: Sale de lista de presupuestos Activos y Genera Orden de Factuarcion y Orden de Pago por cada items asignados a un proveedor sumando los montos de las que corresponden a un mismo proveedor.
        5. Rechazado Sale de lista de Presupuestos Activos, quedando archivado
     2. Fecha Ultima actualizacion
     3. Historial
        1. Consulta
           1. Fecha
           2. Descripción
           3. Respuesta
              1. Fecha
              2. Descripción
     4. Items
     5. Total
     
# Facturación
# Orden de Pago
# Usuarios
1. Personal de la empresa, identificando tareas/departamentos
2. Clientes
3. Proveedores

