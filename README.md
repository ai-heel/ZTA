# ZTA
ZeroTrustArchitecture

## Jawna weryfikacja 
Zawsze przeprowadzaj uwierzytelnianie i autoryzację na podstawie wszystkich dostępnych punktów danych, w tym tożsamości użytkowników, ich lokalizacji, kondycji urządzeń, usługi lub obciążenia, klasyfikacji danych oraz anomalii.
## Korzystanie z dostępu z najniższym poziomem uprawnień
Ogranicz dostęp użytkowników, udzielając go „dokładnie na czas” i tylko w niezbędnym zakresie Just-In-Time (JIT)/Just-Enough-Administration (JEA) oraz stosując zasady adaptacyjne oparte na ryzyku i ochronę danych, aby lepiej zabezpieczyć dane i zadbać o wydajność.
## Podejście „zakładanego naruszenia bezpieczeństwa”
Zminimalizuj obszar zagrożenia i dostęp do segmentów. Weryfikuj kompleksowe szyfrowanie i korzystaj z analiz, aby uzyskać wgląd w informacje, łatwiej wykrywać zagrożenia i wzmocnić mechanizmy obrony.

## Aplikacje 

Aplikacje obejmują systemy, programy komputerowe i usługi, które są wykonywane lokalnie, na urządzeniach mobilnych oraz w środowiskach chmurowych.

Tabela zawiera listę funkcji aplikacji dotyczących ZeroTrust, a także wymagania dotyczące widoczności, analityki, automatyzacji, SDLC oraz zarządzania w kontekście aplikacji.


<!-- Application Access
(Formerly Access
Authorization)
Agency authorizes access to
applications primarily based
on local authorization and
static attributes.
Agency begins to implement
authorizing access
capabilities to applications
that incorporate contextual
information (e.g., identity,
device compliance, and/or
other attributes) per request
with expiration.
Agency automates
application access decisions
with expanded contextual
information and enforced
expiration conditions that
adhere to least privilege
principles.
Agency continuously
authorizes application
access, incorporating real-
time risk analytics and
factors such as behavior or
usage patterns -->
## Uwiezytelnienie i autoryzacja

- 1. Dostęp do aplikacji
na podstawie lokalnej autoryzacji i
statytycznych atrybutów.

- 2. Możliwość autoryzacji dostępu
do aplikacji,
które zawierają kontekstowe
informacje (np. tożsamość,
zgodność urządzenia i/lub
inne atrybuty) na żądanie
z datą wygaśnięcia.

- 3. Automatyczne
decyzje dotyczące
dostępu do aplikacji
z rozszerzonymi
informacjami kontekstowymi i wymuszonymi
warunkami wygaśnięcia, które
przestrzegają zasad
najmniejszych uprawnień.

- 4. Dostęp do
aplikacji wymaga autoryzacji, 
włączając analizę
ryzyka w czasie
rzeczywistym i
czynniki, takie jak wzorce
zachowania i behawiorystyka

<!-- Application Threat
Protections
(Formerly Threat
Protections)
Agency threat protections
have minimal integration
with application workflows,
applying general purpose
Agency integrates threat
protections into mission
critical application
workflows, applying
Agency integrates threat
protections into all
application workflows,
protecting against some
Agency integrates advanced
threat protections into all
application workflows,
offering real-time visibility
Function Traditional Initial Advanced Optimal
protections for known
threats.
protections against known
threats and some application-
specific threats.
application-specific and
targeted threats.
and content-aware
protections against
sophisticated attacks tailored
to applications. -->

## Ochrona przed zagrożeniami

- 1. Aplkacja ma minimalną integrację
z przepływami pracy aplikacji,
stosując ogólnego przeznaczenia

- 2. Firma integruje ochronę
przed zagrożeniami w przepływach
pracy aplikacji o znaczeniu krytycznym, stosując

- 3. Firma integruje ochronę
przed zagrożeniami we wszystkich
przepływach pracy aplikacji,
chroniąc przed niektórymi

- 4. Firma integruje zaawansowaną ochronę
przed zagrożeniami we wszystkich
przepływach pracy aplikacji,
oferując widoczność w czasie rzeczywistym
Funkcja Tradycyjna Początkowa Zaawansowana Optymalna
ochrona przed znanymi
zagrożeniami.
ochrona przed znanymi
zagrożeniami i niektórymi zagrożeniami specyficznymi dla
aplikacji.
zagrożeniami specyficznymi dla
aplikacji i ukierunkowanymi.
oraz ochrona
zależna od treści
przed
zaawansowanymi atakami dostosowanymi
do aplikacji.

<!-- Accessible Applications
(Formerly Accessibility)
Agency makes some mission
critical applications32
available only over private
networks and protected
public network connections
(e.g., VPN) with monitoring.
Agency makes some of their
applicable mission critical
applications available over
open public networks to
authorized users with need
via brokered connections.
Agency makes most of their
applicable mission critical
applications available over
open public network
connections to authorized
users as needed.
Agency makes all applicable
applications available over
open public networks to
authorized users and devices,
where appropriate, as
needed -->

## Ciągłość działania

- 1. Firma udostępnia niektóre
krytyczne dla misji aplikacje32
tylko przez
prywatne
sieci i chronione
publiczne połączenia sieciowe
(np. VPN) z monitorowaniem.

- 2. Firma udostępnia niektóre
swoje krytyczne dla misji aplikacje
przez
otwarte sieci publiczne
upoważnionym użytkownikom z potrzebą
za pośrednictwem pośredniczonych połączeń.

- 3. Firma udostępnia większość
swoich krytycznych dla misji aplikacji
przez
otwarte połączenia sieciowe
upoważnionym użytkownikom w razie potrzeby.
- 4. Firma udostępnia wszystkie
krytyczne dla misji aplikacje
przez
otwarte sieci publiczne
upoważnionym użytkownikom i urządzeniom,
jeśli to stosowne, w razie
potrzeby

<!-- Secure Application
Development and
Deployment Workflow
(New Function)
Agency has ad hoc
development, testing, and
production environments
with non-robust code
deployment mechanisms.
Agency provides
infrastructure for
development, testing, and
production environments
(including automation) with
formal code deployment
mechanisms through CI/CD
pipelines and requisite access
controls in support of least
privilege principles.
Agency uses distinct and
coordinated teams for
development, security, and
operations while removing
developer access to
production environment for
code deployment.
Agency leverages immutable
workloads where feasible,
only allowing changes to
take effect through
redeployment, and removes
administrator access to
deployment environments in
favor of automated processes
for code deployment. -->

## Bezpieczny przepływ pracy rozwoju i wdrożenia aplikacji

- 1. Firma ma ad hoc
środowiska
rozwoju, testowania i
produkcji
z niestabilnymi mechanizmami
wdrażania kodu.
- 2. Firma zapewnia
infrastrukturę dla
środowisk rozwoju, testowania i
produkcji
(w tym automatyzację) z
formalnymi mechanizmami
wdrażania kodu za pośrednictwem
potoków CI/CD i wymaganych
kontroli dostępu w celu
wsparcia zasad najmniejszych uprawnień.
- 3. Firma używa odrębnych i
skoordynowanych zespołów do
rozwoju,
bezpieczeństwa i
operacji, jednocześnie usuwając
dostęp programistów do
środowiska produkcyjnego w celu
wdrażania kodu.
- 4. Firma wykorzystuje niezmienne
obciążenia, gdzie jest to możliwe,
zezwalając na
wprowadzanie zmian tylko poprzez
ponowne wdrożenie i usuwając
dostęp administratora do
środowisk wdrożeniowych na rzecz
zautomatyzowanych procesów
wdrażania kodu.

<!-- Application Security
Testing (Formerly
Application Security)
Agency performs application
security testing prior to
deployment, primarily via
manual testing methods.
Agency begins to use static
and dynamic (i.e.,
application is executing)
testing methods to perform
security testing, including
manual expert analysis, prior
to application deployment.
Agency integrates
application security testing
into the application
development and
deployment process,
including the use of periodic
dynamic testing methods.
Agency integrates
application security testing
throughout the software
development lifecycle across
the enterprise with routine
automated testing of
deployed applications. -->

## Testy bezpieczeństwa aplikacji

- 1. Firma wykonuje testy bezpieczeństwa aplikacji
przed
wdrożeniem, głównie za pomocą
ręcznych metod testowania.
- 2. Firma zaczyna używać statycznych
i dynamicznych (tj.
aplikacja jest wykonywana)
metod testowania, aby wykonywać
testy bezpieczeństwa, w tym
ręczną analizę ekspercką, przed
wdrożeniem aplikacji.
- 3. Firma integruje
testowanie bezpieczeństwa aplikacji
z procesem
rozwoju i
rozwoju aplikacji,
w tym stosowanie okresowych
dynamicznych metod testowania.
- 4. Firma integruje
testowanie bezpieczeństwa aplikacji
w całym
cyklu życia rozwoju oprogramowania w
całym
przedsiębiorstwie z rutynowym
automatyzowanym testowaniem
wdrożonych aplikacji.

<!-- Visibility and Analytics
Capability
Agency performs some
performance and security
monitoring of mission
critical applications with
limited aggregation and
analytics.
Agency begins to automate
application profile (e.g.,
state, health, and
performance) and security
monitoring for improved log
collection, aggregation, and
analytics.
Agency automates profile
and security monitoring for
most applications with
heuristics to identify
application-specific and
enterprise-wide trends and
refines processes over time
to address gaps in visibility.
Agency performs continuous
and dynamic monitoring
across all applications to
maintain enterprise-wide
comprehensive visibility. -->

## Monitorowanie wydajności i bezpieczeństwa

- Firma wykonuje pewne
monitorowanie
wydajności i bezpieczeństwa
aplikacji o znaczeniu krytycznym
z
ograniczoną agregacją i
analityką.
- Firma zaczyna automatyzować
profil aplikacji (np.
stan, kondycję i
wydajność) oraz monitorowanie
bezpieczeństwa w celu poprawy
zbierania,
agregacji i
analityki dzienników.
- Firma automatyzuje monitorowanie
profilu i bezpieczeństwa dla
większości aplikacji za pomocą
heurystyki w celu identyfikacji
trendów specyficznych dla aplikacji i
trendów w całym przedsiębiorstwie oraz
udoskonala procesy w czasie,
aby wyeliminować luki w widoczności.
- Firma wykonuje ciągłe
i dynamiczne monitorowanie
wszystkich aplikacji w celu
utrzymania kompleksowej
widoczności w całym przedsiębiorstwie.

<!-- Automation and
Orchestration Capability
Agency manually establishes
static application hosting
location and access at
provisioning with limited
maintenance and review.
Agency periodically
modifies application
configurations (including
location and access) to meet
relevant security and
performance goals.
Agency automates
application configurations to
respond to operational and
environmental changes.
Agency automates
application configurations to
continuously optimize for
security and performance -->

## Automatyzacja i możliwości orkiestracji

- - Firma ręcznie ustala
statyczną lokalizację
hostingu aplikacji i dostęp przy
zaopatrzeniu z ograniczoną
konserwacją i przeglądem.
- Firma okresowo
modyfikuje konfiguracje
aplikacji (w tym
lokalizację i dostęp), aby
spełnić
odpowiednie cele bezpieczeństwa i
wydajności.
- Firma automatyzuje
konfiguracje aplikacji, aby
reagować na zmiany operacyjne i
środowiskowe.
- Firma automatyzuje
konfiguracje aplikacji, aby
ciągle optymalizować pod kątem
bezpieczeństwa i wydajności

<!-- Governance Capability Agency relies primarily on
manual enforcement policies
for application access,
development, deployment,
software asset management,
security testing and
evaluation (ST&E) at
technology insertion,
patching, and tracking
software dependencies.
Agency begins to automate
policy enforcement for
application development
(including access to
development infrastructure),
deployment, software asset
management, ST&E at
technology insertion,
patching, and tracking
software dependencies based
upon mission needs (for
example, with Software Bill
of Materials).
Agency implements tiered,
tailored policies enterprise-
wide for applications and all
aspects of the application
development and
deployment lifecycles and
leverages automation, where
possible, to support
enforcement.
Agency fully automates
policies governing
applications development
and deployment, including
incorporating dynamic
updates for applications
through the CI/CD pipeline. -->

## Zarządzanie zasobami oprogramowania

- 1. Firma zdolności zarządzania opiera się przede wszystkim na
ręcznych zasadach egzekwowania
dotyczących dostępu do aplikacji,
rozwoju, wdrażania,
zarządzania zasobami oprogramowania,
testowania i
oceny bezpieczeństwa (ST&E) przy
wprowadzaniu technologii,
łataniu i śledzeniu
zależności oprogramowania.
- Firma zaczyna automatyzować
egzekwowanie zasad dla
rozwoju aplikacji
(w tym dostępu do
infrastruktury rozwoju),
wdrażania, zarządzania zasobami oprogramowania, ST&E przy
wprowadzaniu technologii,
łataniu i śledzeniu
zależności oprogramowania w oparciu o
potrzeby misji (na
przykład z zestawieniem
materiałów oprogramowania).
- Firma wdraża wielopoziomowe,
dostosowane zasady w całym przedsiębiorstwie dla aplikacji i wszystkich
aspektów cykli
życia
rozwoju i
wdrażania aplikacji oraz
wykorzystuje automatyzację,
gdzie
to możliwe, w celu
wsparcia egzekwowania. - Firma w pełni automatyzuje
zasady regulujące
rozwój aplikacji
i ich wdrażanie, w tym
włączanie dynamicznych
aktualizacji aplikacji
poprzez proces CI/CD.
