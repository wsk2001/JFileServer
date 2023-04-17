JFileServer - The Java File Server
==================================

Introduction
------------
JFileServer는 현재 SMB/CIFS, FTP/FTPS 및 NFS 프로토콜을 지원하는 Java 기반 파일 서버입니다. 가상 파일 시스템 인터페이스를 사용하면 파일 시스템 메타데이터 및 선택적으로 파일 데이터를 저장하기 위해 데이터베이스를 쉽게 사용할 수 있게 해주는 데이터베이스 파일 시스템 프레임워크를 통해 맞춤형 파일 시스템을 구현할 수 있습니다.

파일 서버는 처리량을 최적화하기 위해 비동기 I/O, 스레드 풀 및 메모리 풀을 사용하여 확장성이 뛰어납니다. Hazelcast 클러스터 기술을 기반으로 추가 확장성을 위해 서버를 클러스터링할 수 있습니다.

엔터프라이즈 애드온 모듈은 SMBv2(고성능) 및 SMBv3(전체 암호화)에 대한 지원을 추가합니다.

History
-------
The JFileServer code originally started out as the JLAN Server, the first version being
released by Starlasoft back in the late 1990's with basic SMB1 support. As development of
the JLAN Server continued, SMB1 support was enhanced, and FTP and NFS support were added,
along with the database filesystem framework and smart caching.

In 2007 Alfresco Software bought the rights to the JLAN Server code rebranding it as Alfresco-JLAN,
and releasing the code as open source. Development continued with the addition of support for 
NTLMv2 and Kerberos enterprise authentication, scaleability enhancements using NIO, thread
pools and memory pools, plus cluster support using Hazelcast, and FTPS support.

In recent years no new development has been done on the Alfresco-JLAN code.

At the beginning of 2018 we forked the Alfresco-JLAN code to create the JFileServer project
to bring the source code up to date, and continue development of the file server.

License
-------
The core JFileServer library and components such as the database filesystem implementations
are licensed under the same GNU LGPL v3.0 license as the original Alfresco-JLAN code.

JDK Version
-----------
The JFileServer code uses features of JDK version 7 onwards.

Docker
------
Pre-configured setups of the core JFileServer and various database fileserver implementations
are available as Docker images which can either be used as they are or used as the starting
point for your own configurations.

For a list of the available Docker images see <https://hub.docker.com/r/filesysorg/>.

Website
-------
The main website can be found at <http://www.filesys.org>.

Additional information and documentation will be added there in the near future.

