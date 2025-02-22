def calcular_descuento(precio, cantidad):
    # Uso de operadores aritméticos (+, *)
    total = precio * cantidad
    descuento = 0
    
    # Uso de operadores relacionales (>, <) y lógicos (and, or)
    if total > 100 and cantidad > 5:
        descuento = total * 0.10  # 10% de descuento
    elif total > 50 or cantidad > 3:
        descuento = total * 0.05  # 5% de descuento
    
    total_final = total - descuento
    return total_final, descuento

# Ejemplo de uso
precio_unitario = float(input("Ingrese el precio unitario del producto: "))
cantidad_comprada = int(input("Ingrese la cantidad comprada: "))

total_a_pagar, descuento_aplicado = calcular_descuento(precio_unitario, cantidad_comprada)
print(f"Total a pagar: {total_a_pagar:.2f}")
print(f"Descuento aplicado: {descuento_aplicado:.2f}")
