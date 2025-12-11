# Discount Calculator

Este proyecto es una calculadora de descuentos escrita en Java. Permite aplicar diferentes códigos de descuento a un precio base y está diseñada para ser utilizada como una biblioteca o componente en aplicaciones más grandes.

## Características

- **Códigos de descuento soportados**:
  - `SAVE10`: Aplica un 10% de descuento.
  - `SUMMER20`: Aplica un 20% de descuento.
  - Otros códigos no afectan el precio.
- Manejo de casos especiales:
  - Precio igual a 0.
  - Códigos de descuento vacíos o nulos.

## Requisitos

- **Java**: Versión 21 o superior.
- **Maven**: Versión 3.9.11 o superior.

## Instalación

1. Clona este repositorio:
   ```bash
   git clone <URL_DEL_REPOSITORIO>
   cd AZ2007
   ```

2. Compila el proyecto con Maven:
   ```bash
   mvn clean install
   ```

## Uso

### Ejemplo de código

```java
import com.example.DiscountCalculator;

public class Main {
    public static void main(String[] args) {
        DiscountCalculator calculator = new DiscountCalculator();
        double price = 100.0;

        double discountedPrice = calculator.applyDiscount(price, "SAVE10");
        System.out.println("Precio con descuento: " + discountedPrice);
    }
}
```

## Pruebas

El proyecto incluye pruebas unitarias para garantizar su correcto funcionamiento. Para ejecutarlas, utiliza el siguiente comando:

```bash
mvn test
```

### Resultados de las pruebas

- **Total de pruebas**: 6
- **Fallos**: 0
- **Errores**: 0
- **Tiempo total**: 0.069 segundos

## Estructura del Proyecto

```
src/
├── main/
│   └── java/
│       └── DiscountCalculator.java
└── test/
    └── java/
        └── DiscountCalculatorTest.java
```

## Dependencias

- **JUnit 5**: Para pruebas unitarias.

## Licencia

Este proyecto está bajo la licencia [MIT](LICENSE).

## Autor

- **Carlo**
