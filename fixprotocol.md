# Useful FIX protocol links

[![Logo](img/fixprotocol.png)](https://www.fixtrading.org)

## Contents
- [Resources](#resources)
    - [FIX Trading Community](#fix-trading-community)
- [Software](#software)
    - [QuickFIX](#quickfix)
    - [ValidFIX](#validfix)

## Resources

### FIX Trading Community

The golden reference source of the FIX protocol information &mdash; specifications, online documentation, community updates, and industry news.

- [Standards](https://www.fixtrading.org/standards/) - a mindmap page for the FIX protocol [body of knowledge](https://en.wikipedia.org/wiki/Body_of_knowledge).
- Formal specifications for session and application FIX protocol levels:
    - [Version 4.4](https://www.fixtrading.org/standards/fix-4-4/) - the most widely adopted version of the FIX protocol.
    - [Version 4.2](https://www.fixtrading.org/standards/fix-4-2/) - another widely adopted (mostly for Equities, FX, and ETFs trading) FIX protocol version.
- [FIX Orchestra](https://www.fixtrading.org/standards/fix-orchestra/) - a Rules-of-Engagement (application-level state machines and messages) specification framework.
- [Repository][fix-repository] - machine-readable specifications suitable for automatic code and documentation generation.
- [FIXimate](http://fiximate.fixtrading.org/latestEP/) - an online FIX protocol reference (generated from the [FIX repository][fix-repository].
- [FIXwiki](http://fixwiki.fixtrading.org/index.php/FIXwiki/) - useful information about all aspects of the FIX protocol, may help digesting relatively dry formal specs.

## Software

### QuickFIX

Reference FIX engine implementations in multiple languages.

Should be the first option to consider &mdash; has a very simple integration API, and a large market of specialists capable of maintaining the original product or an in-house derivative.
Dictionaries, messages, and codecs are generated directly from the [FIX repository][fix-repository].

Is not the fastest or best architected implementation of FIX in the industry, but is so straightfoward, that maintenance and minor adjustments should not be a problem even for an amateur software engineer.

Performance bottlenecks are well known and can be addressed in-house without full rewrite &mdash; excessive dynamic memory allocation, suboptimal codecs, message representation, and data containers.

- [QuickFIX](http://www.quickfixengine.org/) - C++ implementation with Python wrappers [on github](https://github.com/quickfix/quickfix), runs on Linux, Windows, and Mac OS X.
- [QuickFIX/J](https://www.quickfixj.org/) - Java implementation on [github](https://github.com/quickfix-j/quickfixj).
- [quickFIX/n](https://www.quickfixn.org/) - .NET implementation on [github](https://github.com/connamara/quickfixn) by Connamara Systems.
- [QuickFIX/Go](https://www.quickfixgo.org/) - Go implementation on [github](https://github.com/quickfixgo/quickfix).

### ValidFIX

An interactive web-based FIX traffic analyzer. Has enterprise-friendly commercial offering.

- [FIX Analyzer](http://www.validfix.com/fix-analyzer.html) - use to inspect a single FIX message.
- [FIX Log Analyzer](http://www.validfix.com/fix-log-analyzer.html) - use to inspect any section of a log file.


[fix-repository]: https://www.fixtrading.org/standards/fix-repository/
