# Ejercicios finales de repaso

## Explica, en tus propias palabras, por qué es necesario que las computadoras representen los datos en binario.
Las computadoras usan el sistema binario porque funcionan con electricidad, y sus componentes solo pueden tener dos estados: encendido o apagado, que se representan con 1 y 0. Esto hace que el hardware sea más simple, más rápido y menos propenso a errores, ya que solo tiene que reconocer dos niveles de voltaje. Además, con solo esos dos números se puede representar cualquier tipo de dato y hacer cálculos de forma eficiente.

## Convierte el número binario 10011011 a decimal y a hexadecimal.
1×128 + 0×64 + 0×32 + 1×16 + 1×8 + 0×4 + 1×2 + 1×1 = 155
El número binario 10011011 equivale a 155 en decimal
El número binario 10011011 se agrupa en bloques de cuatro bits: 1001 y 1011, que corresponden a 9 y B. Por lo tanto, su equivalente en hexadecimal es 9B.

## Investiga y describe cómo se representa una imagen en formato PNG en el disco.
Un archivo PNG empieza con una firma especial que dice “esto es un PNG” y luego tiene varios bloques llamados chunks. Los más importantes son: IHDR, que guarda cosas como el tamaño y tipo de color; IDAT, donde está la imagen comprimida; y IEND, que marca el final del archivo. Cada bloque tiene info sobre su tamaño, tipo, datos y una especie de chequeo para asegurarse de que no haya errores. También pueden venir otros bloques con cosas extra como colores, transparencia o texto.

## Analiza la siguiente situación: ¿Qué sucede si intentas almacenar un número mayor al que puede representar un byte (por ejemplo, 300)? ¿Cómo lo maneja Python?
Si intentas meter un número más grande de lo que un byte aguanta, no cabe y puede dar error o perder info. En Python los números enteros no tienen límite, así que puedes usar el 300 sin problema. Pero si quieres poner ese número en algo que solo acepta un byte, como un array de bytes, te va a tirar error porque 300 no entra ahí. Básicamente, Python deja manejar números grandes, pero al pasarlos a formatos con límite hay que tener cuidado para no pasarse del rango.