---
title: TiDB Cloud Billing
summary: Learn about TiDB Cloud billing.
---

# TiDB Cloud請求 {#tidb-cloud-billing}

> **ノート：**
>
> [開発者層のクラスター](/tidb-cloud/select-cluster-tier.md#developer-tier)は最大 1 年間無料で使用できます。 Developer Tier クラスターの使用に対して課金されることはなく、 TiDB Cloudの請求書には Developer Tier の料金は表示されません。

TiDB Cloudは、消費したリソースに応じて課金されます。詳細については、 [TiDB Cloudの価格詳細](https://en.pingcap.com/tidb-cloud-pricing-details/)にアクセスしてください。

## 請求書 {#invoices}

組織の所有者または課金管理者であれば、 TiDB Cloudの請求書情報を管理できます。それ以外の場合は、このセクションをスキップしてください。

> **ノート：**
>
> [AWS マーケットプレイス](https://aws.amazon.com/marketplace)からTiDB Cloudにサインアップすると、AWS アカウントから直接支払うことができますが、支払い方法を追加したり、 TiDB Cloudポータルで請求書をダウンロードしたりすることはできません。

支払い方法を設定すると、 TiDB Cloudは毎月の初めに前月の請求書を生成します。請求書のコストには、組織内の TiDB クラスターの使用量、割引、バックアップ ストレージのコスト、サポート サービスのコスト、クレジットの消費、およびデータ転送のコストが含まれます。

-   TiDB Cloudは毎月 9 日に請求書を発行します。 1 日目から 9 日目までは、前月のコストの詳細を表示することはできませんが、課金コンソールを介して今月のクラスターの使用状況情報を取得できます。
-   請求書の支払いのデフォルトの方法は、クレジット カードによる控除です。他の支払い方法を使用したい場合は、チケットリクエストを送信してお知らせください。
-   請求書発行後、30日以内にお支払いを完了してください。
-   今月と前月の料金の概要と詳細を表示できます。

> **ノート：**
>
> すべての請求控除は、サードパーティのプラットフォームである Stripe を通じて行われます。

請求書のリストを表示するには、次の手順を実行します。

1.  TiDB Cloudコンソールの右上隅にあるアカウント名をクリックします。
2.  [**請求]**をクリックします。請求書ページが表示されます。

## 支払明細 {#billing-details}

組織の所有者または請求管理者である場合は、 TiDB Cloudの請求の詳細を表示およびエクスポートできます。それ以外の場合は、このセクションをスキップしてください。

支払い方法を設定した後、 TiDB Cloudは過去の月の請求書と請求の詳細を生成し、各月の初めに当月の請求の詳細を生成します。請求の詳細には、組織の TiDB クラスターの使用量、割引、バックアップ ストレージのコスト、データ転送コスト、サポート サービスのコスト、クレジットの消費、およびプロジェクト分割情報が含まれます。

> **ノート：**
>
> 遅延やその他の理由により、当月の請求明細は参考用であり、正確であることを保証するものではありません。 TiDB Cloudは、原価計算を実行し、他のニーズを満たすことができるように、過去の請求書の正確性を保証します。

請求の詳細を表示するには、次の手順を実行します。

1.  TiDB Cloudコンソールの右上隅にあるアカウント名をクリックします。
2.  [**請求]**をクリックします。
3.  **請求書**をクリックします。請求の詳細ページが表示されます。

## クレジット {#credits}

TiDB Cloudは、概念実証 (PoC) ユーザーに一定数のクレジットを提供します。 1 クレジットは 1 米ドルに相当します。クレジットの有効期限が切れる前に、クレジットを使用して TiDB クラスター料金を支払うことができます。

> **ヒント：**
>
> PoC に申し込むには、 [TiDB Cloudで概念実証 (PoC) を実行する](/tidb-cloud/tidb-cloud-poc.md)を参照してください。

クレジットの詳細情報は、合計クレジット、使用可能なクレジット、現在の使用状況、ステータスなど、**クレジット**ページで確認できます。

このページを表示するには、次の手順を実行します。

1.  TiDB Cloudコンソールの右上隅にあるアカウント名をクリックします。
2.  [**請求]**をクリックします。
3.  [**クレジット]**をクリックします。クレジットの詳細ページが表示されます。

> **ノート：**
>
> -   支払い方法を設定すると、クラスター料金はまず未使用のクレジットから差し引かれ、次に支払い方法から差し引かれます。
> -   サポートプラン料金のお支払いにはクレジットはご利用いただけません。

> **警告：**
>
> PoC プロセス中:
>
> -   支払い方法を追加する前にすべてのクレジットが期限切れになると、新しいクラスターを作成できなくなります。 3 日後、既存のクラスターはすべてリサイクルされます。 7 日後、すべてのバックアップがリサイクルされます。プロセスを再開するには、支払い方法を追加できます。
> -   支払い方法を追加した後にすべてのクレジットが期限切れになった場合、PoC プロセスが続行され、支払い方法から料金が差し引かれます。

## 支払方法 {#payment-method}

組織の所有者または課金管理者であれば、 TiDB Cloudの支払い情報を管理できます。それ以外の場合は、このセクションをスキップしてください。

> **ノート：**
>
> [AWS マーケットプレイス](https://aws.amazon.com/marketplace)からTiDB Cloudにサインアップすると、AWS アカウントから直接支払うことができますが、支払い方法を追加したり、 TiDB Cloudポータルで請求書をダウンロードしたりすることはできません。

### クレジットカードを追加 {#add-a-credit-card}

料金は、クラスターの使用状況に応じて、バインドされたクレジット カードから差し引かれます。有効なクレジット カードを追加するには、次のいずれかの方法を使用できます。

-   クラスターを作成する場合:

    1.  [ **Create a クラスタ** ] ページで [ <strong>Create クラスタ</strong> ] をクリックする前に、[ <strong>Billing Calculator</strong> ] ウィンドウの下部にある [ <strong>Add Credit Card</strong> ] をクリックします。
    2.  [**カードを追加**] ダイアログ ボックスで、カード情報と請求先住所を入力します。
    3.  [**カードを保存]**をクリックします。

-   請求コンソールでいつでも:

    1.  TiDB Cloudコンソールの右上隅にあるアカウント名をクリックします。
    2.  [**請求]**をクリックします。
    3.  [**支払い方法**] タブで、[<strong>新しいカードを追加</strong>] をクリックします。
    4.  請求先住所とカード情報を入力し、[**保存**] をクリックします。

> **ノート：**
>
> クレジット カードの機密データのセキュリティを確保するために、 TiDB Cloudは顧客のクレジット カード情報を保存せず、サードパーティの支払いプラットフォームである Stripe に保存します。すべての課金控除は、Stripe を通じて完了します。

複数のクレジット カードをバインドし、そのうちの 1 つを課金コンソールの支払い方法の既定のクレジット カードとして設定できます。設定後、以降の請求はデフォルトのクレジットカードから自動的に引き落とされます。

デフォルトのクレジット カードを設定するには、次の手順を実行します。

1.  TiDB Cloudコンソールの右上隅にあるアカウント名をクリックします。
2.  [**請求]**をクリックします。
3.  [**お支払い方法**] タブをクリックします。
4.  クレジット カード リストでクレジット カードを選択し、[**既定に設定**] をクリックします。

### 請求プロファイル情報の編集 {#edit-billing-profile-information}

請求プロファイル情報には、会社の正式な住所と税務登録情報が含まれます。税務登録番号を提供することにより、特定の税金が請求書から免除される場合があります。

請求プロファイル情報を編集するには、次の手順を実行します。

1.  TiDB Cloudコンソールの右上隅にあるアカウント名をクリックします。
2.  [**請求]**をクリックします。
3.  [**お支払い方法**] タブをクリックします。
4.  請求プロファイル情報を編集し、[**保存**] をクリックします。