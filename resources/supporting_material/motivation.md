* interconnected world
* IoT needs Security
  * why
* TLS is one such protocol that provides security
  * too expensive for IoT
* Existing work does not evaluate the cost 

# Motivation

In recent years there has been a sharp increase in the number of IoT
devices and this trend is expected to continue. The IoT is a network
of interconnected devices, which exchange data with one another over
the internet. While they are many types of IoT devices, all of them
are restricted: they have limited memory, processing power and
available energy. Examples of IoT devices include temperature sensors,
smart lightbulb and physical activity trackers.

While inter-device communication has numerous benefits, it is important
to ensure the security of that communication. For example, when you log
in to your online banking account, you do not want others to be
able to see your password, as this may lead to the compromise of your
account. Having your account compromised means that a malicious entity
might steal your money. Similarly, when you are transferring funds via
online banking, you want the contents of that operation to be
invisible to an observer, for privacy reasons. It is also desirable
that no party is able to tamper with the transmitted data en transit,
as it may lead to undesired consequences, such as the transfer of a
larger amount than you intended. Proper communications security allows
those goals to be achieved.

TLS is one of the most used protocols for communication security. It
powers numerous technologies, such as HTTPS. TLS offers the
security services of authentication, confidentiality, privacy, integrity, replay
protection and perfect forward secrecy. It is not a requirement to use all of
those services for every TLS connection. The procotol is similar to
a frmework, in the sense that you can enable individual security
services on a per-connection basis. For example, when you are downloading
software updates, data confidentiality is probably not a concern,
data authenticity and integrity, however, is. In TLS, it is possible for a connection
to only offer authenticity and integirty, without offering confidentiality.
Foregoing unecessary serivices will lead to a smaller reseouce usage,
which in turn leads to smaller execution time and power usage. This
is especially important in the context of IoT, due to the constrained
nature of the devices.

There are numerous IoT devices, each one with different hardware
capabilities and security requirements. For example, some IoT
devices have the capability of using public key cryptography,
while for others symmetric cryptography is the only option
In some cases, the communicating devices require data authenticity, confidentiality
and integrity (e.g. when logging in into a device), while in others data
authenticity and integrity is enough (e.g. when transferring updates).

TLS was not designed for the constrained environment of IoT. Despite that,
it is a malleable protocol and can be configured to one's needs. In essence,
it is a combination of various security algorithms that together form
a protocol for communication secuirty. If configured
properly, it is possible to use it in the context of IoT. Existing work
does not address the computational cost evaluation of the various security services
offered by TLS individually. This computational cost can be the number of CPU
instructions used, time taken or power used. For this reason, software developers
that want to use TLS to provide connection security do not have data that can
assist them in making the security/resouce usage trade-offs.

The goal of this work is to evaluate the cost of each security service of the
TLS protocol. This will assit software developers to make security/resouce usage
tradeoff judments, according to their needs and limitations. For this reason,
this work targeted towards developers who whish to add communication security
to their applications in the IoT environment.
