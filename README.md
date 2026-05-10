**Fase 1: Infraestructura Técnica (Base del Equipo)
Este es el "paso 0" para que nadie pierda trabajo al usar GitHub.

[ ] Configurar Git LFS: Activar el rastreo de archivos pesados (.uasset, .umap).

[ ] Establecer el .gitignore: Bloquear carpetas temporales (Intermediate, Saved).

[ ] Estructura de Carpetas: Crear carpetas estándar: /Content/FastFoodSim/Blueprints/Core y /UI.

[ ] Definir la moneda: Decidir si usarán números enteros (Céntimos: 1050) o decimales (Floats: 10.50). Recomendación: Usar Floats para facilidad.

Fase 2: El Cerebro Económico (Lógica)
Aquí es donde el código decide qué pasa con el dinero.

[ ] Crear S_OrderData (Struct): Definir qué información lleva un pedido (ID, Nombre, CostoComida, PagoCliente, MetodoPago).

[ ] Crear BPC_EconomyManager (Actor Component):

[ ] Variable CashWallet (Efectivo).

[ ] Variable BankBalance (App FFod).

[ ] Función AddTransaction: Que reciba el monto y el tipo (Cash/Bank) y actualice los saldos.

[ ] Sistema de Liquidación de Deuda: Lógica para que al cobrar en efectivo, el sistema descuente el costo de la comida de la cuenta bancaria del jugador.

Fase 3: La App FFod e Interacción (Mecánicas)
Hacer que el sistema se sienta como "Schedule 1".

[ ] Interface de Interacción (BPI_Interactable): Para que el jugador pueda tocar cajeros o terminales de pago.

[ ] Lógica de Cajero (ATM):

[ ] Función DepositCash.

[ ] Función WithdrawCash.

[ ] Generador de Pedidos: Un sistema simple que cree pedidos aleatorios basados en el S_OrderData y los envíe a la App.

Fase 4: Interfaz de Usuario (UI)
Lo que el jugador ve en su teléfono.

[ ] Widget Base del Teléfono: Diseño de la pantalla principal.

[ ] Pantalla de Wallet: Visualización en tiempo real de CashWallet y BankBalance.

[ ] Notificación de Pago: Un mensaje visual cada vez que se completa un pedido ("+$15.00 recibidos").

[ ] Resumen del Día: Pantalla que aparece al terminar el turno mostrando:

Ingresos Totales.

Costos de Comida.

Ganancia Neta.

Fase 5: Estabilidad y Pulido (Testing)
[ ] Protección contra Saldo Negativo: Evitar que el jugador retire más dinero del que tiene en el banco.

[ ] Persistencia (Save System): Lograr que al cerrar el juego y volver a abrirlo, el dinero se mantenga.

[ ] Debug Menu: Crear un comando de consola para sumarse dinero y probar la economía rápidamente.**
