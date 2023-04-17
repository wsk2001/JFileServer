JFileServer - The Java File Server
==================================

Introduction
------------
JFileServer는 현재 SMB/CIFS, FTP/FTPS 및 NFS 프로토콜을 지원하는 Java 기반 파일 서버입니다. 가상 파일 시스템 인터페이스를 사용하면 파일 시스템 메타데이터 및 선택적으로 파일 데이터를 저장하기 위해 데이터베이스를 쉽게 사용할 수 있게 해주는 데이터베이스 파일 시스템 프레임워크를 통해 맞춤형 파일 시스템을 구현할 수 있습니다.

파일 서버는 처리량을 최적화하기 위해 비동기 I/O, 스레드 풀 및 메모리 풀을 사용하여 확장성이 뛰어납니다. Hazelcast 클러스터 기술을 기반으로 추가 확장성을 위해 서버를 클러스터링할 수 있습니다.

<span style="color:blue"> **엔터프라이즈 애드온 모듈은 SMBv2(고성능) 및 SMBv3(전체 암호화)에 대한 지원을 추가합니다.** </span>

History
-------
JFileServer 코드는 원래 JLAN 서버로 시작했으며, 기본 SMB1 지원과 함께 1990년대 후반에 Starlasoft에서 첫 번째 버전을 출시했습니다. JLAN 서버의 개발이 계속됨에 따라 SMB1 지원이 향상되었고 FTP 및 NFS 지원이 데이터베이스 파일 시스템 프레임워크 및 스마트 캐싱과 함께 추가되었습니다.

2007년 Alfresco Software는 JLAN 서버 코드에 대한 권리를 구입하여 Alfresco-JLAN으로 리브랜딩하고 코드를 오픈 소스로 공개했습니다. NTLMv2 및 Kerberos 엔터프라이즈 인증에 대한 지원, NIO를 사용한 확장성 향상, 스레드 풀 및 메모리 풀, Hazelcast를 사용한 클러스터 지원, FTPS 지원을 추가하여 개발이 계속되었습니다.

최근 몇 년 동안 Alfresco-JLAN 코드에 대한 새로운 개발이 이루어지지 않았습니다.

2018년 초에 Alfresco-JLAN 코드를 포크하여 JFileServer 프로젝트를 생성하여 소스 코드를 최신 상태로 유지하고 파일 서버 개발을 계속했습니다.

License
-------
핵심 JFileServer 라이브러리 및 데이터베이스 파일 시스템 구현과 같은 구성 요소는 원래 Alfresco-JLAN 코드와 동일한 GNU LGPL v3.0 라이선스에 따라 라이선스가 부여됩니다.

JDK Version
-----------
JFileServer 코드는 JDK 버전 7 이후의 기능을 사용합니다.

Docker
------
Pre-configured setups of the core JFileServer and various database fileserver implementations
are available as Docker images which can either be used as they are or used as the starting
point for your own configurations.

For a list of the available Docker images see <https://hub.docker.com/r/filesysorg/>.

Website
-------
기본 웹사이트는 <http://www.filesys.org> 에서 찾을 수 있습니다.

가까운 시일 내에 추가 정보와 문서가 추가될 예정입니다.

