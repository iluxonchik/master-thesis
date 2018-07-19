* interconnected world
* IoT needs Security
  * why
* TLS is one such protocol that provides security
  * too expensive for IoT

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
might steal your money. Similarly, when you transferring funds via
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
services on a per-connection basis. For example, 

The issue is that TLS
was not designed for the constrained environment of IoT. Despite that,
it is malleable and can be configured to ones needs. If configured
properly, it is possible to use it in the context of IoT.

There are numerous IoT devices, each one with different hardware
capabilities and security requirements. For example, some IoT
devices have the capability of using public key cryptography,
while for others symmetric cryptography is the only option
In some cases, the communicating devices require data authenticity, confidentiality
and integrity (e.g. when logging in into a device), while in others data
authenticity and integrity is enough (e.g. when transferring updates).
