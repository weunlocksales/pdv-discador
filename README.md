Discador PDV
Discador de PDV con el Phone Widget de comOS. Es una sola página (index.html), sin build ni dependencias que instalar.
Cómo funciona
* Se abre desde el tablero (Apps Script) en una ventana nueva. El tablero le manda la lista de sellers ya filtrada por postMessage.
* Modo Manual: el agente navega la lista y llama a cada número.
* Modo Automático: termina todos los números de un seller (con los intentos y esperas configurados) antes de pasar al siguiente.
* Guarda en el navegador, solo por el día: intentos por número, sellers contactados y las llamadas de hoy.
* Las transcripciones, el audio y las llamadas anteriores los pide el tablero a comOS.
Qué hay que tener en cuenta al mantenerlo
* Carga el script del widget desde https://widget.llamadapro.app/widgetsdk.umd.js con el id de integración pdv-unlock.
* Solo acepta mensajes de orígenes https://*-script.googleusercontent.com. Si el tablero se publica en otro dominio, hay que ajustar esa validación en el listener de message.
* La sección Pruebas permite llamar a un número propio o armar una cola de prueba (varios sellers separados por coma; varios teléfonos por seller separados por ;).
Publicación
Es una página estática: sirve cualquier hosting estático (por ejemplo GitHub Pages).
