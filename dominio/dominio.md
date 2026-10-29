# Configuración de Dominio Personalizado y Certificado SSL/TLS / Custom Domain & SSL/TLS Certificate Setup

---

## 🇪🇸 Español

### Descripción General
Documentación del proceso de delegación de DNS con **Namecheap** y **AWS Route 53**, además de la emisión y validación de certificados SSL/TLS con **AWS ACM** para habilitar el protocolo HTTPS en `osidevexplorer.me`.

### Pasos de Configuración

#### 1. Delegación DNS (Namecheap a Route 53)
- Se creó una **Hosted Zone** pública en Route 53 para el dominio `osidevexplorer.me`.
- Se obtuvieron los 4 servidores de nombres (*Name Servers - NS*) asignados por AWS.
- En el panel de Namecheap, se configuraron los **Custom DNS** apuntando a los NS de Route 53.

#### 2. Certificado SSL/TLS (AWS Certificate Manager)
- Solicitud de certificado público para `osidevexplorer.me` y `*.osidevexplorer.me`.
- Validación mediante registros **CNAME** añadidos automáticamente en Route 53.
- Estado del certificado: **Issued** (Emitido).

#### 3. Configuración del Listener HTTPS (443) y Enrutamiento Alias
- Se agregó el Listener **HTTPS:443** en el ALB (`osi-dev-alb`) asociando el certificado emitido.
- Se creó un registro de tipo **A (Alias)** en Route 53 apuntando el dominio raíz directamente al Application Load Balancer en la región `us-east-2`.

### Verificación
El dominio `https://osidevexplorer.me` resuelve correctamente con conexión segura mediante HTTPS.

---

## 🇬🇧 English

### Overview
Documentation of the DNS delegation process using **Namecheap** and **AWS Route 53**, along with the issuance and validation of SSL/TLS certificates via **AWS ACM** to enable HTTPS for `osidevexplorer.me`.

### Configuration Steps

#### 1. DNS Delegation (Namecheap to Route 53)
- Created a public **Hosted Zone** in Route 53 for the domain `osidevexplorer.me`.
- Obtained the 4 Name Servers (NS) assigned by AWS.
- Configured **Custom DNS** in Namecheap pointing to the Route 53 NS servers.

#### 2. SSL/TLS Certificate (AWS Certificate Manager)
- Requested a public certificate for `osidevexplorer.me` and `*.osidevexplorer.me`.
- Validated via **CNAME** records automatically added to Route 53.
- Certificate status: **Issued**.

#### 3. HTTPS (443) Listener & Alias Routing Setup
- Added an **HTTPS:443** listener to the ALB (`osi-dev-alb`) attaching the issued certificate.
- Created an **A (Alias)** record in Route 53 pointing the root domain directly to the Application Load Balancer in region `us-east-2`.

### Verification
The domain `https://osidevexplorer.me` resolves successfully over a secure HTTPS connection.