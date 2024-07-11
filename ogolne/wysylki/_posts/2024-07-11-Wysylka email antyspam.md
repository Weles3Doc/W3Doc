---
title: Wysyłka e-mail - Anty-spam
---

# Wysyłka e-mail — Anty-spam

Bezpośrednio nie mamy wpływu na filtry antyspamowe używane przez dostawców skrzynek do filtrowania przychodzących wiadomości mailowych. Opisane tutaj punkty mają za zadanie zwiększyć dostarczalność maili wysyłanych przez `Weles3`, przez Państwa domenę i serwer. Są to ustawienia, które należy wprowadzić dla swojej domeny, w której znajduje się konto/konta pocztowe używane do wysyłki wiadomości z `Weles3`. Wymagana jest własna domena, nie można zmienić tych parametrów np. dla kont `Gmail`.

#### Klikanie "To nie spam".

Zachęcenie właścicieli do oznaczania wiadomości "To nie spam" lub podobnie. Powinno to zaktualizować indywidualny filtry danego właściciela, przyszłe wiadomości nie będą oznaczane jako spam. Może spowodować, że dostawca poczty właściciela uzna mailingi z Państwa domeny za wiarygodne.

#### Wpis DKIM

W ustawieniach Państwa domeny  (na stronie dostawcy domeny) mogą Państwo dodać wpis:

`w3._domainkey IN CNAME w3.domainkey.e-adm.pl.`

KIM służy do uwierzytelniania wysyłanej wiadomości e-mail. System przed rozpoczęciem wysyłki sprawdza, czy ten wpis jest poprawny i jeżeli tak to podpisuje wiadomości e-mail.

#### Wpis SPF

W ustawieniach Państwa domeny (na stronie dostawcy domeny) mogą Państwo dodać wpis:

`IN TXT "v=spf1 mx ~all"`

SPF wskazuje serwery poczty uprawnione do wysyłania e-maili w imieniu Twojej domeny.

#### Wpis DMARC

W ustawieniach Państwa domeny (na stronie dostawcy domeny) mogą Państwo dodać wpis:

`_dmarc IN TXT "v=DMARC1; p=none; adkim=s; aspf=s; rua=mailto:[adres e-mail do raportów]"`

W miejsce [adres e-mail do raportów] podstawiamy adres mail, na który mają być wysyłane zbiorcze raporty o działaniach DMARC. DMARC jest protokołem uwierzytelniania, zasad i raportowania poczty e-mail.

#### Instrukcja

Niestety nie wskażemy tutaj dokładnego postępowania, ponieważ kroki, jakie należy podjąć, zależą od dostawcy domeny.

Przykłady dla HOME.PL:

- [DKIM](https://pomoc.home.pl/baza-wiedzy/dkim-uwierzytelnianie-poczty-e-mail-rekord-txt)
- [SPF](https://pomoc.home.pl/baza-wiedzy/co-to-jest-rekord-spf-domeny)
- [DMARC](https://pomoc.home.pl/baza-wiedzy/dmarc-co-to-jest-i-jak-dziala-jak-ustawic-rekord-dmarc-w-panelu-klienta)

Przykład dla OVH:

- [DKIM](https://help.ovhcloud.com/csm/pl-dns-zone-dkim?id=kb_article_view&sysparm_article=KB0058254)
- [SPF](https://help.ovhcloud.com/csm/pl-dns-spf-record?id=kb_article_view&sysparm_article=KB0051716)
- [DMARC](https://help.ovhcloud.com/csm/pl-dns-zone-dmarc?id=kb_article_view&sysparm_article=KB0061459)