# taximetro_mgr
Proyecto Taxímetro Factoría F5
"""
Fase 1: Solicitud de servicio
"""
print("Bienvenidos a x. Somos la unica empresa de transportes que ofrece serrvicio a familias con niños")
nombre_padre_o_madre = input("Indicame el nombre del padre o madre que solicita el servicio"" ")
nombre_niño = input(f"¡Genial! {nombre_padre_o_madre}, ahora dime el nombre de tu hijo o hija: ")

#Condicional para verificar si necesita silla de bebé
silla_bebe = input("¿Tu hijo es menor de 12 años? (si/no)").lower()
if silla_bebe == "si":
    print((nombre_niño), "necesita una silla de niños, según las normas del DGT.¡No te preocupes! La llevarémos por ti sin costo adicional")
elif silla_bebe == "no":
    print("Perfecto, no es necesario llevar silla de niños")
else:
    print("No te entendí. Por favor responde si o no.")
    
# Bucle para repetir la pregunta
while silla_bebe not in ["si","no"]:
    silla_bebe = input("¿Tu hijo es menor de 12 años? (si/no)").lower()
    if silla_bebe == "si":
        print((nombre_niño), "necesita una silla de niños, según las normas del DGT.¡No te preocupes! La llevarémos por ti sin costo adicional")
    elif silla_bebe == "no":
        print("Perfecto, no es necesario llevar silla de niños")
    else:
        print("No te entendí. Por favor responde si o no.")

# Origen y Destino 
punto_partida = input("Dime a qué lugar debe ir nuestro conductor a recogerlos"" ")
destino = input("¿A qué lugar van a ir? (Por favor, dime la ubicación de ese lugar"" ")
dis_kilometros = input( "¿A cuántos kilómetros queda desde el punto de partida?"" ")

# Velocidad de movimiento
print("Nos ajustamos a tu ritmo: elige la velocidad que les dé tranquilidad a ti y a tu hijo.")
velocidad_elegida = input("Elige una velocidad (Rápido/Normal/Lento)").lower()
if velocidad_elegida == "rápido":
    velocidad = 100  # km/h
    print("¡Genial! Vamos a ir rápido.")
elif velocidad_elegida == "normal":
    velocidad = 60  # km/h
    print("¡Perfecto! Vamos a ir a una velocidad normal.")
elif velocidad_elegida == "lento":
    velocidad = 30  # km/h
    print("¡Muy bien! Vamos a ir despacio.")
else:
    print("No te entendí. Por favor, elige entre rápido, normal o lento.")



    
