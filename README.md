# Jayway: Tu Pasaporte a los Mejores Servicios

Jayway es tu plataforma todo en uno para acceder a una amplia gama de servicios de alta calidad, desde barberías hasta gimnasios y más, todo en un solo lugar.

## Barber Hub: Donde el Estilo se Encuentra con la Comodidad

Barber Hub es tu destino único para encontrar los mejores servicios de barbería en tu área. Con Barber Hub, puedes descubrir las barberías más destacadas, reservar citas de manera fácil y disfrutar de un corte de cabello excepcional en el lugar que más te guste. Ya sea que busques un corte clásico o un estilo moderno, en Barber Hub encontrarás todo lo que necesitas para mantenerte a la vanguardia de la moda.

### Distribución de Ganancias para Barber Hub (30 Suscripciones, Costo de Suscripción de 30 soles)

| Parte            | Porcentaje (%) | Ganancia Mensual por Cliente | Ganancia Total Mensual |
|------------------|----------------|-------------------------------|------------------------|
| Persona Jurídica (Negocio) |      67.75     |          20.325 soles         |        609.75 soles      |
| Jayway (Plataforma)         |      32.25     |             9.675 soles      |        290.25 soles      |

### Distribución de Ganancias para Barber Hub (160 Suscripciones, Costo de Suscripción de 30 soles)

| Parte            | Porcentaje (%) | Ganancia Mensual por Cliente | Ganancia Total Mensual |
|------------------|----------------|-------------------------------|------------------------|
| Persona Jurídica (Negocio) |      67.75     |          20.325 soles         |        3252 soles      |
| Jayway (Plataforma)         |      32.25     |             9.675 soles      |        1548 soles      |


## Gym Hub: Tu Centro de Bienestar Personal

Gym Hub es tu centro de bienestar personal, donde puedes encontrar los mejores gimnasios y centros de entrenamiento en tu área. Con Gym Hub, puedes explorar una variedad de opciones de entrenamiento, desde pesas hasta clases de yoga, y encontrar el lugar perfecto para alcanzar tus metas de fitness. Ya sea que seas un principiante o un atleta experimentado, en Gym Hub encontrarás todo lo que necesitas para mantenerte en forma y saludable.

## Distribución de Ganancias para Gimnasios (Rango de 30 a 60 Suscripciones, Costo de Suscripción entre 80 y 120 soles)

### Para el Costo de Suscripción de 80 Soles

| Parte            | Porcentaje (%) | Ganancia Mensual por Cliente (mínimo) | Ganancia Mensual por Cliente (máximo) | Ganancia Total Mensual (mínima) | Ganancia Total Mensual (máxima) |
|------------------|----------------|----------------------------------------|----------------------------------------|----------------------------------|----------------------------------|
| Persona Jurídica (Negocio) |      70.00     |                    56                  |                56                    |        1680                     |      3360                       |
| Jayway (Plataforma)         |      30.00     |                      24                      |            24                        |            720                  |          1440                     |

### Para el Costo de Suscripción de 120 Soles

| Parte            | Porcentaje (%) | Ganancia Mensual por Cliente (mínimo) | Ganancia Mensual por Cliente (máximo) | Ganancia Total Mensual (mínima) | Ganancia Total Mensual (máxima) |
|------------------|----------------|----------------------------------------|----------------------------------------|----------------------------------|----------------------------------|
| Persona Jurídica (Negocio) |      70.00     |                    84                  |                84                    |        2520                     |      5040                       |
| Jayway (Plataforma)         |      30.00     |                      36                      |            36                        |            1080                 |          2160                     |

Únete a Jayway hoy y descubre por qué somos la opción preferida para aquellos que buscan comodidad y calidad en sus servicios diarios.

## Modelado de Datos

### Modelo de Entidad Afiliada (Affiliated Entity)

```json
{
  "_id": "entityAffiliateId",
  "corporateName": "Corporate Name",
  "entityType": "Type of Entity",
  "documentNumber": "XXXXXX",
  "documentType": "ID/Passport",
  "responsible": "Responsible Name",
  "phones": [
    {
      "type": "Cellphone/Landline",
      "number": "XXXXXX"
    }
  ],
  "city": "City",
  "country": "Country",
  "businessSector": "Business Sector"
}
```
### Modelo de Suscripciones de Cliente (Customer Subscription)

```json
{
  "_id": "customerSubscriptionId",
  "customerId": "customerId",
  "entityAffiliateId": "entityAffiliateId",
  "subscriptionName": "Annual Plus Plan",
  "subscriptionTypeId": "subscriptionTypeId",
  "startDate": "2024-01-01",
  "expirationDate": "2024-12-31",
  "pricePaid": "1200",
  "features": [
    "Unlimited access to all facilities",
    "4 personal training sessions per month"
  ],
  "status": "Active"
}
```

### Modelo de Pagos de Suscripción (Subscription Payment)

```json
{
  "_id": "paymentId",
  "customerSubscriptionId": "customerSubscriptionId",
  "paymentDate": "2024-01-01",
  "amount": "1200",
  "paymentMethod": "Credit Card",
  "status": "Completed",
  "details": "Payment for annual Plus Plan"
}
```

### Modelo de Clientes (Customer)

```json
{
  "_id": "customerId",
  "fullName": "Customer Full Name",
  "documentNumber": "XXXXXX",
  "documentType": "ID/Passport",
  "profilePicture": "URL of Profile Picture",
  "address": "Customer Address",
  "email": "Customer Email",
  "phone": "Customer Phone Number",
  "dateOfBirth": "Customer Date of Birth",
  "gender": "Customer Gender",
  "interests": [
    "Interest 1",
    "Interest 2"
  ],
  "subscriptions": [
    // List of customer subscriptions
  ]
}
```

