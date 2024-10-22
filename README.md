# cines
print("")
print("                                  ✩✩✩CINE✩✩✩")
print("")
#Menú de combos # your own code
print("✩COMBOS:")
print("")
print("1)COMBO TRADICIONAL-------$230\n 1 Palomitas Grandes Clasicas + 2 Refrescos Grandes\n")
print("2) COMBO NACHOS-------------$233\n 1 Palomitas Grandes Clasicas + 1 Refresco Grande + 1 Nachos Clasicos\n")
print("3) COMBO GRANDE-------------$190\n 1 Palomitas Grandes Clasicas + 1 Refresco Grande + 1 pza Milky Way 48g o 1 pza Snickers 48g\n ")
print("4) COMBO HOT DOG------------$247\n 1 Palomitas Grandes Clasicas + 1 Refresco Grande + 1 Hot Dog Clasico\n")
print("5) COMBO ICEE------------------$292\n 1 Palomitas Grandes Clasicas + 2 ICEE + 1 M&Ms (49.3g)\n")
print("6) COMBO KITKAT----------------$199\n 1 Palomitas Grandes+2 Refrescos Grandes+1 Kitkat\n")
print("7) COMBO VASOS COLECCIONABLES--$315\n 1 Palomitas Grandes+2 Vasos Grandes con refresco\n")
#validación del combo (si es verdadero) # your own code
combo = int(input("Ingrese el número relacionado al combo que desee comprar: "))
if combo >= 1 and combo <= 7:
  #entrada de datos con relacion a la cantidad de combos que desea comprar # your own code
  cantidad = int(input("Ingrese la cantidad de combos que desea"))
  #validación de la cantidad de combos (si es verdadero) # your own code
  if cantidad > 0:
    #entrada de datos con relacion a la cantidad de combos, guardar el precio y nombre para la impresión del ticket # your own code
    if combo == 1:
      multi = cantidad * 230
      comboF = "Combo tradicional"
      precio = 230
    elif combo == 2:
      multi = cantidad * 233
      comboF = "Combo nachos"
      precio = 233
    elif combo == 3:
      multi = cantidad * 190
      comboF = "Combo Grande"
      precio = 190
    elif combo == 4:
      multi = cantidad * 247
      comboF = "Combo Hot Dogs"
      precio = 247
    elif combo == 5:
      multi = cantidad * 292
      comboF = "Combo Icee"
      precio = 292
    elif combo == 6:
      multi = cantidad * 199
      comboF = "Combo KitKat"
      precio = 199
    else:
      multi = cantidad * 315
      comboF = "Combo Vasos Coleccionables"
      precio = 315
    preguntaMembre = str(input("¿Cuentas con alguna membresia? (si/no): "))
    #Validación de si se cuenta con membresia (verdadero) # your own code
    if preguntaMembre == "si" or preguntaMembre == "SI" or preguntaMembre == "Si":
      #Impresion de un menú de membresias # your own code
      print("TIPOS DE MEMBRESIAS")
      print("1)Estandar")
      print("2)Oro")
      print("3)Platino")
      #entrada de datos del tipo de membresia del cliente # your own code
      membresia = int(input("Ingrese el tipo de membresia con la que cuenta"))
      #validacion de la membresia # your own code
      if membresia > 0 and membresia < 4:
        #cascada para calcular los descuentos y almacenar la membresia parala impresion # your own code
        if membresia == 1:
          descuen = multi * 0.01
          mem = "Estandar"
        elif membresia == 2:
          descuen = multi * 0.05
          mem = "Oro"
        elif membresia == 3:
          descuen = multi * 0.10
          mem = "Platino"
      else:
        #Validacion de la membresia (falso) # your own code
        print("Membresia inexistente")
    else:
      #en caso de no contar con membresia # your own code
      descuen = 0
      mem = "Sin membresia"
    #Se calcula el total a pagar incluyendo el descuento # your own code
    total = multi - descuen
    #salida de datos # your own code
    print("")
    print("-"*30)
    print("        DATOS DE COMPRA")
    print("-"*30)
    print("COMBO\t      ",comboF)
    print("PRECIO\t             ", precio)
    print("CANTIDAD\t      ",cantidad)
    print("-"*30)
    print("MEMBRESIA\t      ",mem)
    print("-"*30)
    print("TOTAL\t             ",multi)
    print("DESCUENTO\t      ",descuen)
    print("TOTAL FINAL DE SU COMPRA   ",total)
    print("-"*30)
    print("    ¡¡GRACIAS POR SU COMPRA!!")
    print("     ¡DISFRUTE SU FUNCIÓN!")
    print("-"*30)
  #validacion de la cantidad de combos(falso) # your own code
  else:
    print("Combo inexistente")
print("✩✩✩✩✩✩✩✩✩✩✩✩✩✩✩✩✩✩✩✩✩✩✩✩✩✩✩✩✩✩✩✩✩✩✩✩✩✩✩✩✩✩✩✩✩✩✩✩✩✩✩✩✩")
