# Template customization


## src
I hope you have seen this template `src` folder on the downloaded package `Hostbit – Angular 12 Domain Hosting Provider Template` from ThemeForest.

In this `src` folder you can see `index.html` file. This file structure is like this-

```html
<!DOCTYPE html>
<html lang="en">
<head>
  <!--meta, title, base, google fonts, all css linking here-->
</head>

<body>

  <app-root></app-root>
 
 <!--all js linking here-->
</body>

</html>
```

All HTML content will be load into this `app-root`:
```html
<app-root></app-root>
```


## entry points

##### app-component.html
Template `app-component.html` structure looks like this-
```html
<router-outlet></router-outlet>

```

##### app-component.ts
Here we have generated all of our components. Template `app-component.ts` structure looks like this-
```js
import { Component } from '@angular/core';

@Component({
  selector: 'app-root',
  templateUrl: './app.component.html',
  styleUrls: ['./app.component.sass']
})
export class AppComponent {
  title = 'hostbit';
}

```

##### app.module.ts
Template `app.module.ts` structure looks like this-
```js
import { NgModule } from '@angular/core';
import { BrowserModule } from '@angular/platform-browser';

import { AppRoutingModule } from './app-routing.module';
import { AppComponent } from './app.component';
import { ThemeOneComponent } from './themes/theme-one/theme-one.component';
import { HeroComponent } from './components/hero/hero.component';
import { PromoOneComponent } from './components/promo/promo-one/promo-one.component';
import { PromoTwoComponent } from './components/promo/promo-two/promo-two.component';
import { PromoThreeComponent } from './components/promo/promo-three/promo-three.component';
import { ContentOneComponent } from './components/content/content-one/content-one.component';
import { ContentTwoComponent } from './components/content/content-two/content-two.component';
import { ContentThreeComponent } from './components/content/content-three/content-three.component';
import { ContentFourComponent } from './components/content/content-four/content-four.component';
import { ContentFiveComponent } from './components/content/content-five/content-five.component';
import { ContentSixComponent } from './components/content/content-six/content-six.component';
import { ServiceOneComponent } from './components/service/service-one/service-one.component';
import { ServiceTwoComponent } from './components/service/service-two/service-two.component';
import { PricingOneComponent } from './components/pricing/pricing-one/pricing-one.component';
import { PricingTwoComponent } from './components/pricing/pricing-two/pricing-two.component';
import { ReviewOneComponent } from './components/review/review-one/review-one.component';
import { ReviewTwoComponent } from './components/review/review-two/review-two.component';
import { CtaOneComponent } from './components/cta/cta-one/cta-one.component';
import { CtaTwoComponent } from './components/cta/cta-two/cta-two.component';
import { DataCenterOneComponent } from './components/data-center/data-center-one/data-center-one.component';
import { DataCenterTwoComponent } from './components/data-center/data-center-two/data-center-two.component';
import { FooterComponent } from './components/footer/footer.component';
import { HeaderComponent } from './components/header/header.component';
import { ScrollupComponent } from './components/scrollup/scrollup.component';
import { ModalSearchComponent } from './components/modal/modal-search/modal-search.component';
import { ModalMenuComponent } from './components/modal/modal-menu/modal-menu.component';
import { BreadcrumbWordpressComponent } from './components/breadcrumb/breadcrumb-wordpress/breadcrumb-wordpress.component';
import { BreadcrumbEcommerceComponent } from './components/breadcrumb/breadcrumb-ecommerce/breadcrumb-ecommerce.component';
import { BreadcrumbSharedComponent } from './components/breadcrumb/breadcrumb-shared/breadcrumb-shared.component';
import { BreadcrumbVpsComponent } from './components/breadcrumb/breadcrumb-vps/breadcrumb-vps.component';
import { BreadcrumbEmailComponent } from './components/breadcrumb/breadcrumb-email/breadcrumb-email.component';
import { BreadcrumbDedicatedComponent } from './components/breadcrumb/breadcrumb-dedicated/breadcrumb-dedicated.component';
import { BreadcrumbCloudComponent } from './components/breadcrumb/breadcrumb-cloud/breadcrumb-cloud.component';
import { BreadcrumbResellerComponent } from './components/breadcrumb/breadcrumb-reseller/breadcrumb-reseller.component';
import { BreadcrumbDomainCheckerComponent } from './components/breadcrumb/breadcrumb-domain-checker/breadcrumb-domain-checker.component';
import { BreadcrumbDomainTransferComponent } from './components/breadcrumb/breadcrumb-domain-transfer/breadcrumb-domain-transfer.component';
import { HostingWordpressComponent } from './components/hosting/hosting-wordpress/hosting-wordpress.component';
import { HostingEcommerceComponent } from './components/hosting/hosting-ecommerce/hosting-ecommerce.component';
import { HostingSharedComponent } from './components/hosting/hosting-shared/hosting-shared.component';
import { HostingVpsComponent } from './components/hosting/hosting-vps/hosting-vps.component';
import { HostingEmailComponent } from './components/hosting/hosting-email/hosting-email.component';
import { HostingDedicatedComponent } from './components/hosting/hosting-dedicated/hosting-dedicated.component';
import { HostingCloudComponent } from './components/hosting/hosting-cloud/hosting-cloud.component';
import { HostingResellerComponent } from './components/hosting/hosting-reseller/hosting-reseller.component';
import { DomainSearchComponent } from './components/domain/domain-search/domain-search.component';
import { DomainCheckerComponent } from './components/domain/domain-checker/domain-checker.component';
import { DomainTransferComponent } from './components/domain/domain-transfer/domain-transfer.component';
import { BreadcrumbDataCenterComponent } from './components/breadcrumb/breadcrumb-data-center/breadcrumb-data-center.component';
import { FaqOneComponent } from './components/faq/faq-one/faq-one.component';
import { FaqTwoComponent } from './components/faq/faq-two/faq-two.component';
import { PricingThreeComponent } from './components/pricing/pricing-three/pricing-three.component';
import { PricingFourComponent } from './components/pricing/pricing-four/pricing-four.component';
import { PricingFiveComponent } from './components/pricing/pricing-five/pricing-five.component';
import { PricingSixComponent } from './components/pricing/pricing-six/pricing-six.component';
import { PricingSevenComponent } from './components/pricing/pricing-seven/pricing-seven.component';
import { PricingEightComponent } from './components/pricing/pricing-eight/pricing-eight.component';
import { PricingNineComponent } from './components/pricing/pricing-nine/pricing-nine.component';
import { FaqThreeComponent } from './components/faq/faq-three/faq-three.component';
import { FaqFourComponent } from './components/faq/faq-four/faq-four.component';
import { FaqFiveComponent } from './components/faq/faq-five/faq-five.component';
import { FaqSixComponent } from './components/faq/faq-six/faq-six.component';
import { FaqSevenComponent } from './components/faq/faq-seven/faq-seven.component';
import { ServiceThreeComponent } from './components/service/service-three/service-three.component';
import { CtaThreeComponent } from './components/cta/cta-three/cta-three.component';
import { FeaturesOneComponent } from './components/features/features-one/features-one.component';
import { FeaturesTwoComponent } from './components/features/features-two/features-two.component';
import { ReviewThreeComponent } from './components/review/review-three/review-three.component';
import { FeaturesThreeComponent } from './components/features/features-three/features-three.component';
import { ContentSevenComponent } from './components/content/content-seven/content-seven.component';
import { ContentEightComponent } from './components/content/content-eight/content-eight.component';
import { ContentNineComponent } from './components/content/content-nine/content-nine.component';
import { ServiceFourComponent } from './components/service/service-four/service-four.component';
import { PromoFourComponent } from './components/promo/promo-four/promo-four.component';
import { CenterComponent } from './components/data-center/center/center.component';

@NgModule({
  declarations: [
    AppComponent,
    ThemeOneComponent,
    HeroComponent,
    PromoOneComponent,
    PromoTwoComponent,
    PromoThreeComponent,
    ContentOneComponent,
    ContentTwoComponent,
    ContentThreeComponent,
    ContentFourComponent,
    ContentFiveComponent,
    ContentSixComponent,
    ServiceOneComponent,
    ServiceTwoComponent,
    PricingOneComponent,
    PricingTwoComponent,
    ReviewOneComponent,
    ReviewTwoComponent,
    CtaOneComponent,
    CtaTwoComponent,
    DataCenterOneComponent,
    DataCenterTwoComponent,
    FooterComponent,
    HeaderComponent,
    ScrollupComponent,
    ModalSearchComponent,
    ModalMenuComponent,
    BreadcrumbWordpressComponent,
    BreadcrumbEcommerceComponent,
    BreadcrumbSharedComponent,
    BreadcrumbVpsComponent,
    BreadcrumbEmailComponent,
    BreadcrumbDedicatedComponent,
    BreadcrumbCloudComponent,
    BreadcrumbResellerComponent,
    BreadcrumbDomainCheckerComponent,
    BreadcrumbDomainTransferComponent,
    HostingWordpressComponent,
    HostingEcommerceComponent,
    HostingSharedComponent,
    HostingVpsComponent,
    HostingEmailComponent,
    HostingDedicatedComponent,
    HostingCloudComponent,
    HostingResellerComponent,
    DomainSearchComponent,
    DomainCheckerComponent,
    DomainTransferComponent,
    BreadcrumbDataCenterComponent,
    FaqOneComponent,
    FaqTwoComponent,
    PricingThreeComponent,
    PricingFourComponent,
    PricingFiveComponent,
    PricingSixComponent,
    PricingSevenComponent,
    PricingEightComponent,
    PricingNineComponent,
    FaqThreeComponent,
    FaqFourComponent,
    FaqFiveComponent,
    FaqSixComponent,
    FaqSevenComponent,
    ServiceThreeComponent,
    CtaThreeComponent,
    FeaturesOneComponent,
    FeaturesTwoComponent,
    ReviewThreeComponent,
    FeaturesThreeComponent,
    ContentSevenComponent,
    ContentEightComponent,
    ContentNineComponent,
    ServiceFourComponent,
    PromoFourComponent,
    CenterComponent
  ],
  imports: [
    BrowserModule,
    AppRoutingModule
  ],
  providers: [],
  bootstrap: [AppComponent]
})
export class AppModule { }

```


## themes

`themes` folder included on `app` folder. You can check our folder structure on `app` folder menu.
This is `themes` folder structure-
```text
|-- themes
    |-- theme-one ( default theme)
```

`themes` folder contains the main demo of Hostbit.


## app-routing
In `app` folder we used `app-routing.module.ts`. Where we linked all the route for our all theme. For routing we used angular-router.

Routes: `src/app/app-routing.module.ts`

```js
import { NgModule } from '@angular/core';
import { RouterModule, Routes } from '@angular/router';
import { ThemeOneComponent } from './themes/theme-one/theme-one.component';
import { HostingWordpressComponent } from './components/hosting/hosting-wordpress/hosting-wordpress.component';
import { HostingEcommerceComponent } from './components/hosting/hosting-ecommerce/hosting-ecommerce.component';
import { HostingSharedComponent } from './components/hosting/hosting-shared/hosting-shared.component';
import { HostingVpsComponent } from './components/hosting/hosting-vps/hosting-vps.component';
import { HostingEmailComponent } from './components/hosting/hosting-email/hosting-email.component';
import { HostingDedicatedComponent } from './components/hosting/hosting-dedicated/hosting-dedicated.component';
import { HostingCloudComponent } from './components/hosting/hosting-cloud/hosting-cloud.component';
import { HostingResellerComponent } from './components/hosting/hosting-reseller/hosting-reseller.component';
import { DomainCheckerComponent } from './components/domain/domain-checker/domain-checker.component';
import { DomainTransferComponent } from './components/domain/domain-transfer/domain-transfer.component';
import { CenterComponent } from './components/data-center/center/center.component';

const routes: Routes = [
  {path: '', component: ThemeOneComponent},
  {path: 'hosting-wordpress', component: HostingWordpressComponent},
  {path: 'hosting-ecommerce', component: HostingEcommerceComponent},
  {path: 'hosting-shared', component: HostingSharedComponent},
  {path: 'hosting-vps', component: HostingVpsComponent},
  {path: 'hosting-email', component: HostingEmailComponent},
  {path: 'hosting-dedicated', component: HostingDedicatedComponent},
  {path: 'hosting-cloud', component: HostingCloudComponent},
  {path: 'hosting-reseller', component: HostingResellerComponent},
  {path: 'domain-checker', component: DomainCheckerComponent},
  {path: 'domain-transfer', component: DomainTransferComponent},
  {path: 'data-center', component: CenterComponent},
];

@NgModule({
  imports: [RouterModule.forRoot(routes)],
  exports: [RouterModule]
})
export class AppRoutingModule { }

```


## components
Under `components` folder we generated all of our components individually. 
We have generated these components to make the developer’s life easy. 
By using these basic components, For example in our components directory there is `header`, `hero` , `hosting` folder where we wrote our different styled component. For example `hero` component-

### Component folder structure
```text
|-- components
    ....
    ..
    |-- header ( header component folder )
    |-- hero ( hero component folder )
    |-- hosting ( hosting component folder )
        - hosting-cloud ( cloud hosting section )
        - hosting-dedicated ( dedicated hosting section )
        ...... ( and other )
    ...    
```


## theme installtion
To install the theme you have to install [angular](https://cli.angular.io/) than go to the theme root dir where `package.json` located and use
```bash
npm install -g @angular/cli
```
it will install the packages.

After install process now you can run local server- local server port is 'http://localhost:4200' For developement start use
```bash
ng serve -o
```
## Build your theme
```bash
ng build --prod
```

## For deployment -- static server
First install
```bash
ng build --watch
ng build --aot
```
If you want to know more about static deployment please visit [Angular app deployment](https://angular.io/guide/deployment)

Enjoy your theme :)
