### Authority 権　限

This publication has been developed by NIST in accordance with its statutory responsibilities under the Federal Information Security Modernization Act (FISMA) of 2014, 44 U.S.C. § 3551 et seq., Public Law(P.L.) 113-283.  
本書は、2014 年連邦情報セキュリティ近代化法（FISMA）、44 U.S.C.§ 3551 et seq.、公法（P.L.）113-283 の下での法定責任に基づき、NIST が作成したものです。 

NIST is responsible for developing information security standards and guidelines, includingminimum requirements for federal information systems, but such standards and guidelines shall not applyto national security systems without the express approval of appropriate federal officials exercising policyauthority over such systems.  
NIST は、連邦政府の情報システムに対する最低限の要件を含む情報セキュリティの基準とガイドラインを策定する責任を負いますが、このような基準とガイドラインは、そのようなシステムに対する政策権限を行使する適切な連邦政府職員の明示的な承認なしには、国家安全保障システムには適用されないものとします。 

This guideline is consistent with the requirements of the Office of Managementand Budget (OMB) Circular A-130.  
本ガイドラインは、Office of Management and Budget (OMB)のCircular A-130の要求事項と一致しています。  

<br>

Nothing in this publication should be taken to contradict the standards and guidelines made mandatory and binding on federal agencies by the Secretary of Commerce under statutory authority.  
本書のいかなる内容も、法令上の権限の下で商務長官が連邦政府機関に対して強制的かつ拘束力のあるものとした基準やガイドラインと矛盾するものであってはなりません。

Nor should these guidelines be interpreted as altering or superseding the existing authorities of the Secretary of Commerce, Director of the OMB, or any other federal official.  
また、これらのガイドラインは、商務長官、OMB長官、またはその他の連邦政府職員の既存の権限を変更したり、それに取って代わるものと解釈されるべきではありません。 

This publication may be used by nongovernmental organizations on a voluntary basis and is not subject to copyright in the United States.  
本書は、非政府組織が任意で使用することができ、米国における著作権の対象ではありません。 

Attribution would, however, be appreciated by NIST.  
しかし、NIST は帰属表示を歓迎します。  
<br/>

Certain commercial entities, equipment, or materials may be identified in this document in order to describe an experimental procedure or concept adequately.   
本書では、実験手順や概念を適切に記述するために、ある種の市販の事業体、機器、または材料を特定している場合がある。  

Such identification is not intended to imply recommendation or endorsement by NIST, nor is it intended to imply that the entities, materials, or equipment are necessarily the best available for the purpose.  
このような特定は、NISTによる推奨や推奨を意味するものではなく、また、そのような事業体、材料、または装置が必ずしもその目的のために利用可能な最善のものであることを意味するものでもない。  

There may be references in this publication to other publications currently under development by NIST in accordance with its assigned statutory responsibilities.  
本書の中には、NISTが割り当てられた法定責任に従って現在開発中の他の出版物への言及がある場合がある。 

The information in this publication, including concepts and methodologies, may be used by Federal agencies even before the completion of such companion publications.  
概念や方法論を含む本書の情報は、そのような関連出版物が完成する前であっても、連邦機関によって使用される可能性がある。

Thus, until each publication is completed, current requirements, guidelines, and procedures, where they exist, remain operative.  
したがって、各出版物が完成するまでは、現在の要求事項、ガイドラインおよび手順が存在する場合には、その内容が有効である。

For planning and transition purposes, Federal agencies may wish to closely follow the development of these new publications by NIST.  
計画と移行の目的のために、連邦機関は、NISTによるこれらの新出版物の開発を注視することを推奨する。
<br>

※  
Organizations are encouraged to review all draft publications during public comment periods and provide feedback to NIST. 
組織は、パブリックコメント期間中にすべての出版物の草案を検討し、NIST にフィードバックを提供することが推奨される。

Many NIST cybersecurity publications, other than the ones noted above, are available at https://csrc.nist.gov/publications.
上記以外の多くのNISTサイバーセキュリティ関連の出版物は、https://csrc.nist.gov/publications で入手可能である。  

※訳者注：本文書はdraftのため、最後の２文の表記が少し変化しています。  

<br>

### Reports on Computer Systems Technology
### コンピュータシステム技術に関するレポート

The Information Technology Laboratory (ITL) at the National Institute of Standards and Technology (NIST) promotes the U.S. economy and public welfare by providing technical leadership for the Nation’s measurement and standards infrastructure.  
国立標準技術研究所(NIST)の情報技術研究所(ITL)は、国家の測定・標準インフラストラクチャに技術的なリーダーシップを提供することで、米国経済と公共の福祉を促進しています。 

ITL develops tests, test methods, reference data, proof of concept implementations, and technical analyses to advance the development and productive use of information technology.  
ITLは、情報技術の開発と生産的な利用を促進するために、試験、試験方法、参照データ、概念実証の実装、技術分析を開発しています。 

ITL’s responsibilities include the development of management, administrative, technical, and physical standards and guidelines for the cost-effective security and privacy of other than national security-related information in federal information systems.  
ITLの責任には、連邦政府の情報システムにおける国家安全保障関連情報以外の情報の費用対効果の高いセキュリティとプライバシーのための管理、管理、技術、物理的な標準およびガイドラインの開発が含まれています。 

The Special Publication 800-series reports on ITL’s research, guidelines, and outreach efforts in information system security, and its collaborative activities with industry, government, and academic organizations.  
特別刊行物800シリーズは、情報システム・セキュリティにおけるITLの研究、ガイドライン、アウトリーチ活動、および産業界、政府、学術機関との協力活動について報告しています。

<br/>

### Abstract 
### 抄　録

Zero trust (ZT) is the term for an evolving set of cybersecurity paradigms that move network defenses from static, network-based perimeters to focus on users, assets, and resources.  
ゼロ・トラスト（ZT）とは、ネットワークの防御を静的なネットワークベースの境界線から、ユーザー、資産、およびリソースに焦点を当てたものへと移行させる、進化するサイバーセキュリティのパラダイムのセットを指す用語です。 

A zero trust architecture (ZTA) uses zero trust principles to plan enterprise infrastructure and workflows.  
ゼロ・トラスト・アーキテクチャ（ZTA）は、企業のインフラストラクチャとワークフローを計画するためにゼロ・トラストの原則を使用します。 

Zero trust assumes there is no implicit trust granted to assets or user accounts based solely on their physical or network location (i.e., local area networks versus the internet).  
ゼロ・トラストでは、物理的なロケーションやネットワーク上のロケーション（例えば、ＬＡＮやインターネットなど）のみに基づいている暗黙の信頼は資産やユーザー・アカウントに付与されないことを前提としています。 

Authentication and authorization (both user and device) are discrete functions performed before a session to an enterprise resource is established.  
認証と認可（ユーザーとデバイスの両方）は、企業リソースへのセッションが確立される前に実行される個別の機能です。 

Zero trust is a response to enterprise network trends that include remote users and cloud-based assets that are not located within an enterprise- owned network boundary.  
ゼロトラストは、企業が所有するネットワーク境界内には存在しないリモートユーザーやクラウドベースの資産を含む企業ネットワークのトレンドに対応しています。

Zero trust focus on protecting resources, not network segments, as the network location is no longer seen as the prime component to the security posture of the resource.  
ゼロトラストはネットワークセグメントではなく、リソースの保護に焦点を当てており、ネットワークのロケーションがリソースのセキュリティ態勢の主要な要素であるとは考えられなくなっています。 

This document contains an abstract definition of zero trust architecture (ZTA) and gives general deployment models and use cases where zero trust could improve an enterprise’s overall information technology security posture.
この文書では、ゼロ・トラスト・アーキテクチャ（ZTA）の抽象的な定義を含み、ゼロ・トラストが企業の全体的な情報技術セキュリティ態勢を改善する可能性のある一般的な展開モデルとユースケースを示しています。

<br/>

### Keywords 
### キーワード

architecture; cybersecurity; enterprise; network security; zero trust.  
アーキテクチャ、サイバーセキュリティ、エンタープライズ、ネットワークセキュリティ、ゼロトラスト  

<br/>

### Acknowledgments
### 謝　辞

This document is the product of a collaboration between multiple federal agencies and is overseen by the Federal CIO Council.  
このドキュメントは、複数の連邦政府機関間の共同作業の成果物であり、連邦 CIO 評議会によって監督されています。 

The architecture subgroup is responsible for development of this document, but there are specific individuals who deserve recognition.  
このドキュメントの開発はアーキテクチャ・サブグループが担当していますが、評価に値する特定の人物がいます。 

These include Greg Holden, project manager of the Federal CIO Council ZTA project; Alper Kerman, project manager for the NIST/National Cybersecurity Center of Excellence ZTA effort; and Douglas Montgomery.  
Federal CIO Council ZTA プロジェクトのプロジェクト・マネージャーである Greg Holden 氏、NIST/National Cybersecurity Center of Excellence ZTA 取り組みのプロジェクト・マネージャーである Alper Kerman 氏、そして Douglas Montgomery 氏です。

<br/>

### Audience 
### 対象者

This document is intended to describe zero trust for enterprise security architects.  
この文書は、企業のセキュリティアーキテクト向けにゼロトラストを説明することを目的としています。 

It is meant to aid understanding of zero trust for civilian unclassified systems and provide a road map to migrate and deploy zero trust security concepts to an enterprise environment.  
民間の未分類システムに対するゼロトラストの理解を助け、ゼロトラストセキュリティの概念をエンタープライズ環境に移行して展開するためのロードマップを提供することを意図しています。 

Agency cybersecurity managers, network administrators, and managers may also gain insight into zero trust and ZTA from this document.  
機関のサイバーセキュリティ管理者、ネットワーク管理者、管理者は、この文書からゼロトラストと ZTAについての洞察を得ることができます。

It is not intended to be a single deployment plan for ZTA as an enterprise will have unique business use cases and data assets that require protection.  
企業には、保護を必要とする独自のビジネスユースケースやデータ資産があるため、ZTAの単一の展開計画を意図したものではありません。

Starting with a solid understanding of the organization’s business and data will result in a strong approach to zero trust.  
組織のビジネスとデータをしっかりと理解することから始めることで、ゼロトラストへの強力なアプローチが可能になります。

<br/>

### Note to Reviewers 
### レビュアーへの注意事項 

The purpose of this Special Publication is to develop a technology-neutral set of terms, definitions, and logical architectural components to develop and support a ZTA.  
この特別出版物の目的は、ZTA を開発し、サポートするための技術的に中立な用語、定義および論理的なアーキテクチャコンポーネントのセットを開発することです。 

This document does not give specific guidance or recommendations on how to deploy zero trust components in an enterprise.  
この文書は、企業内にゼロトラストコンポーネントを展開する方法について、具体的なガイダンスや推奨事項を提供するものではありません。

Reviewers are asked to tailor their comments based on the stated purpose of the document.  
レビュアーは、この文書の目的に基づいてコメントを調整することが求められます。

<br/>

### Trademark Information  
### 商標情報

All registered trademarks or trademarks belong to heir respective organizations.  
すべての登録商標または商標は、それぞれの組織に帰属します。