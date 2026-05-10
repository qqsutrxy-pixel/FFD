🛵 Fast Food Simulator (Codename: FFod)
Fast Food Simulator es un simulador de repartos desarrollado en Unreal Engine 5.1. El jugador asume el rol de un repartidor independiente que debe gestionar sus pedidos, su economía física/digital y el mantenimiento de su equipo a través de la app FFod.

🚀 Estado del Proyecto: Fase de Cimentación
Actualmente, el equipo está trabajando en el núcleo del sistema económico y la integración de la infraestructura en GitHub.

💰 Sistema de Economía (Propuesta Técnica)
El juego utiliza un sistema de flujo de caja dual inspirado en simuladores de gestión inmersiva:

1. Tipos de Fondos
Cartera Física (Cash): Dinero recibido por pedidos en efectivo. Se usa para gastos rápidos y depósitos en cajeros.

Banca Digital (FFod App): Dinero recibido por tarjetas o transferencias. Es el saldo disponible para retiros y pagos oficiales de la app.

2. Lógica de Transacción
Para cada pedido, se calcula el beneficio real restando el costo del producto:

Fórmula: Ganancia Neta = (Precio Cliente + Propina) - Costo de Comida

Al final de cada jornada laboral, el sistema genera un Resumen de Liquidación para mostrar la rentabilidad del jugador.

🛠️ Guía para Colaboradores
Requisitos Previos
Unreal Engine 5.1.x instalado.

Git LFS (Obligatorio). Antes de clonar, ejecuta:

Bash
git lfs install
Visual Studio 2022 (con soporte para C++ de Unreal).

Flujo de Trabajo
Ramas (Branches): No trabajes directamente en main. Crea una rama con tu nombre o tarea: feature/sistema-dinero.

Blueprints: Antes de editar un Blueprint importante, avisa por el canal de comunicación para evitar conflictos de mezcla (Merge Conflicts).

Source Control: Activa el "Source Control" dentro del editor de Unreal para ver quién tiene bloqueado cada archivo.

📝 Lista de Tareas (Roadmap)
Fase 1: Core & GitHub
[x] Configuración de Repositorio y Colaboradores.

[ ] Creación de .gitignore y Git LFS.

[ ] Estructura de carpetas inicial (/Content/FFod/Core).

Fase 2: Lógica Económica
[ ] Implementar Struct S_OrderData.

[ ] Desarrollar BPC_EconomyManager (Componente de Actor).

[ ] Sistema de interacción con ATMs (Cajeros).

Fase 3: Interfaz (App FFod)
[ ] Diseño de Widget base para el teléfono.

[ ] Pantalla de gestión de finanzas.

[ ] Notificaciones de pago recibido.

👥 Integrantes
[Usuarios] - Hunter Valtherion / Bytyrrexx_ / ⏃ 𝕯𝖊𝖑𝖋𝖎𝖓𝕬𝖔𝖎 ⏃ / Foxsee / Buru Buru ブルブル

[Colaboradores] - Gameplay -- 

💡 Nota sobre Copyright
El nombre "Fast Food Simulator" y la app "FFod" son nombres en clave provisionales para evitar infracciones de propiedad intelectual relacionadas con marcas de delivery reales.
