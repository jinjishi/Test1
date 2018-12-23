# Test1
/*==============================================================*/
/* DBMS name:      Sybase SQL Anywhere 11                       */
/* Created on:     2018/12/23 22:40:34                          */
/*==============================================================*/


if exists(select 1 from sys.sysforeignkey where role='FK_ADD_ADD_SHOPPING') then
    alter table "Add"
       delete foreign key FK_ADD_ADD_SHOPPING
end if;

if exists(select 1 from sys.sysforeignkey where role='FK_ADD_ADD2_PRODUCT') then
    alter table "Add"
       delete foreign key FK_ADD_ADD2_PRODUCT
end if;

if exists(select 1 from sys.sysforeignkey where role='FK_ADDRESS_UA_USER') then
    alter table Address
       delete foreign key FK_ADDRESS_UA_USER
end if;

if exists(select 1 from sys.sysforeignkey where role='FK_BS_BS_BRAND') then
    alter table BS
       delete foreign key FK_BS_BS_BRAND
end if;

if exists(select 1 from sys.sysforeignkey where role='FK_BS_BS2_STORE') then
    alter table BS
       delete foreign key FK_BS_BS2_STORE
end if;

if exists(select 1 from sys.sysforeignkey where role='FK_BELONG_BELONG_STORE') then
    alter table Belong
       delete foreign key FK_BELONG_BELONG_STORE
end if;

if exists(select 1 from sys.sysforeignkey where role='FK_BELONG_BELONG2_PRODUCT') then
    alter table Belong
       delete foreign key FK_BELONG_BELONG2_PRODUCT
end if;

if exists(select 1 from sys.sysforeignkey where role='FK_CARE_CARE_STORE') then
    alter table Care
       delete foreign key FK_CARE_CARE_STORE
end if;

if exists(select 1 from sys.sysforeignkey where role='FK_CARE_CARE2_USER') then
    alter table Care
       delete foreign key FK_CARE_CARE2_USER
end if;

if exists(select 1 from sys.sysforeignkey where role='FK_LANDING_QL_QQ') then
    alter table Landing
       delete foreign key FK_LANDING_QL_QQ
end if;

if exists(select 1 from sys.sysforeignkey where role='FK_LANDING_UL_USER') then
    alter table Landing
       delete foreign key FK_LANDING_UL_USER
end if;

if exists(select 1 from sys.sysforeignkey where role='FK_LANDING_WL2_WECHAT') then
    alter table Landing
       delete foreign key FK_LANDING_WL2_WECHAT
end if;

if exists(select 1 from sys.sysforeignkey where role='FK_ORDER_AO_ADDRESS') then
    alter table "Order"
       delete foreign key FK_ORDER_AO_ADDRESS
end if;

if exists(select 1 from sys.sysforeignkey where role='FK_ORDER_OU_USER') then
    alter table "Order"
       delete foreign key FK_ORDER_OU_USER
end if;

if exists(select 1 from sys.sysforeignkey where role='FK_PO_PO_PRODUCT') then
    alter table PO
       delete foreign key FK_PO_PO_PRODUCT
end if;

if exists(select 1 from sys.sysforeignkey where role='FK_PO_PO2_ORDER') then
    alter table PO
       delete foreign key FK_PO_PO2_ORDER
end if;

if exists(select 1 from sys.sysforeignkey where role='FK_PURCHASE_PURCHASE_PRODUCT') then
    alter table Purchase
       delete foreign key FK_PURCHASE_PURCHASE_PRODUCT
end if;

if exists(select 1 from sys.sysforeignkey where role='FK_PURCHASE_PURCHASE2_USER') then
    alter table Purchase
       delete foreign key FK_PURCHASE_PURCHASE2_USER
end if;

if exists(select 1 from sys.sysforeignkey where role='FK_QQ_QL2_LANDING') then
    alter table QQ
       delete foreign key FK_QQ_QL2_LANDING
end if;

if exists(select 1 from sys.sysforeignkey where role='FK_SHOPPING_VISIT2_USER') then
    alter table Shoppingcar
       delete foreign key FK_SHOPPING_VISIT2_USER
end if;

if exists(select 1 from sys.sysforeignkey where role='FK_USER_UL2_LANDING') then
    alter table "User"
       delete foreign key FK_USER_UL2_LANDING
end if;

if exists(select 1 from sys.sysforeignkey where role='FK_USER_VISIT_SHOPPING') then
    alter table "User"
       delete foreign key FK_USER_VISIT_SHOPPING
end if;

if exists(select 1 from sys.sysforeignkey where role='FK_WECHAT_WL_LANDING') then
    alter table WeChat
       delete foreign key FK_WECHAT_WL_LANDING
end if;

if exists(
   select 1 from sys.systable 
   where table_name='Add'
     and table_type in ('BASE', 'GBL TEMP')
) then
    drop table "Add"
end if;

if exists(
   select 1 from sys.systable 
   where table_name='Address'
     and table_type in ('BASE', 'GBL TEMP')
) then
    drop table Address
end if;

if exists(
   select 1 from sys.systable 
   where table_name='BS'
     and table_type in ('BASE', 'GBL TEMP')
) then
    drop table BS
end if;

if exists(
   select 1 from sys.systable 
   where table_name='Belong'
     and table_type in ('BASE', 'GBL TEMP')
) then
    drop table Belong
end if;

if exists(
   select 1 from sys.systable 
   where table_name='Brand'
     and table_type in ('BASE', 'GBL TEMP')
) then
    drop table Brand
end if;

if exists(
   select 1 from sys.systable 
   where table_name='Care'
     and table_type in ('BASE', 'GBL TEMP')
) then
    drop table Care
end if;

if exists(
   select 1 from sys.systable 
   where table_name='Landing'
     and table_type in ('BASE', 'GBL TEMP')
) then
    drop table Landing
end if;

if exists(
   select 1 from sys.systable 
   where table_name='Order'
     and table_type in ('BASE', 'GBL TEMP')
) then
    drop table "Order"
end if;

if exists(
   select 1 from sys.systable 
   where table_name='PO'
     and table_type in ('BASE', 'GBL TEMP')
) then
    drop table PO
end if;

if exists(
   select 1 from sys.systable 
   where table_name='Product'
     and table_type in ('BASE', 'GBL TEMP')
) then
    drop table Product
end if;

if exists(
   select 1 from sys.systable 
   where table_name='Purchase'
     and table_type in ('BASE', 'GBL TEMP')
) then
    drop table Purchase
end if;

if exists(
   select 1 from sys.systable 
   where table_name='QQ'
     and table_type in ('BASE', 'GBL TEMP')
) then
    drop table QQ
end if;

if exists(
   select 1 from sys.systable 
   where table_name='Shoppingcar'
     and table_type in ('BASE', 'GBL TEMP')
) then
    drop table Shoppingcar
end if;

if exists(
   select 1 from sys.systable 
   where table_name='Store'
     and table_type in ('BASE', 'GBL TEMP')
) then
    drop table Store
end if;

if exists(
   select 1 from sys.systable 
   where table_name='User'
     and table_type in ('BASE', 'GBL TEMP')
) then
    drop table "User"
end if;

if exists(
   select 1 from sys.systable 
   where table_name='WeChat'
     and table_type in ('BASE', 'GBL TEMP')
) then
    drop table WeChat
end if;

/*==============================================================*/
/* Table: "Add"                                                 */
/*==============================================================*/
create table "Add" 
(
   "Time"               timestamp                      not null,
   Productid            char(20)                       not null,
   Color                char(10)                       not null,
   Size                 char(10)                       not null,
   constraint PK_ADD primary key ("Time", Productid, Color, Size)
);

/*==============================================================*/
/* Table: Address                                               */
/*==============================================================*/
create table Address 
(
   Consignee            varchar(50)                    not null,
   Phone                integer                        not null,
   Address              varchar(100)                   not null,
   Userid               char(20)                       not null,
   constraint PK_ADDRESS primary key (Consignee, Address)
);

/*==============================================================*/
/* Table: BS                                                    */
/*==============================================================*/
create table BS 
(
   Brandid              char(20)                       not null,
   Storeid              char(20)                       not null,
   constraint PK_BS primary key (Brandid, Storeid)
);

/*==============================================================*/
/* Table: Belong                                                */
/*==============================================================*/
create table Belong 
(
   Storeid              char(20)                       not null,
   Productid            char(20)                       not null,
   Color                char(10)                       not null,
   Size                 char(10)                       not null,
   constraint PK_BELONG primary key (Storeid, Productid, Color, Size)
);

/*==============================================================*/
/* Table: Brand                                                 */
/*==============================================================*/
create table Brand 
(
   Brandid              char(20)                       not null,
   Brandname            varchar(50)                    not null,
   constraint PK_BRAND primary key (Brandid)
);

/*==============================================================*/
/* Table: Care                                                  */
/*==============================================================*/
create table Care 
(
   Storeid              char(20)                       not null,
   Userid               char(20)                       not null,
   constraint PK_CARE primary key (Storeid, Userid)
);

/*==============================================================*/
/* Table: Landing                                               */
/*==============================================================*/
create table Landing 
(
   Password             char(20)                       not null,
   Userid               char(20)                       null,
   QQid                 char(20)                       null,
   Weid                 char(20)                       null,
   constraint PK_LANDING primary key (Password)
);

/*==============================================================*/
/* Table: "Order"                                               */
/*==============================================================*/
create table "Order" 
(
   Orderid              integer                        not null,
   Consignee            varchar(50)                    not null,
   Address              varchar(100)                   not null,
   Userid               char(20)                       not null,
   "Date"               timestamp                      not null,
   Condition            char(20)                       not null,
   constraint PK_ORDER primary key (Orderid)
);

/*==============================================================*/
/* Table: PO                                                    */
/*==============================================================*/
create table PO 
(
   Productid            char(20)                       not null,
   Color                char(10)                       not null,
   Size                 char(10)                       not null,
   Orderid              integer                        not null,
   constraint PK_PO primary key (Productid, Color, Size, Orderid)
);

/*==============================================================*/
/* Table: Product                                               */
/*==============================================================*/
create table Product 
(
   Productid            char(20)                       not null,
   Productname          varchar(100)                   not null,
   Price                numeric(10)                    not null,
   Inventory            integer                        not null,
   "Comment"            integer                        not null,
   Salesvolume          integer                        not null,
   Postage              numeric(10)                    not null,
   Color                char(10)                       not null,
   Weight               decimal(10)                    null,
   Size                 char(10)                       not null,
   constraint PK_PRODUCT primary key (Productid, Color, Size)
);

/*==============================================================*/
/* Table: Purchase                                              */
/*==============================================================*/
create table Purchase 
(
   Productid            char(20)                       not null,
   Color                char(10)                       not null,
   Size                 char(10)                       not null,
   Userid               char(20)                       not null,
   constraint PK_PURCHASE primary key (Productid, Color, Size, Userid)
);

/*==============================================================*/
/* Table: QQ                                                    */
/*==============================================================*/
create table QQ 
(
   QQid                 char(20)                       not null,
   QQpassword           char(20)                       not null,
   constraint PK_QQ primary key (QQid)
);

/*==============================================================*/
/* Table: Shoppingcar                                           */
/*==============================================================*/
create table Shoppingcar 
(
   "Time"               timestamp                      not null,
   Userid               char(20)                       null,
   constraint PK_SHOPPINGCAR primary key ("Time")
);

/*==============================================================*/
/* Table: Store                                                 */
/*==============================================================*/
create table Store 
(
   Storeid              char(20)                       not null,
   Storename            varchar(50)                    not null,
   constraint PK_STORE primary key (Storeid)
);

/*==============================================================*/
/* Table: "User"                                                */
/*==============================================================*/
create table "User" 
(
   Userid               char(20)                       not null,
   Nickname             varchar(50)                    not null,
   Sex                  char(2)                        not null,
   constraint PK_USER primary key (Userid)
);

/*==============================================================*/
/* Table: WeChat                                                */
/*==============================================================*/
create table WeChat 
(
   Weid                 char(20)                       not null,
   WePassword           char(20)                       not null,
   constraint PK_WECHAT primary key (Weid)
);

alter table "Add"
   add constraint FK_ADD_ADD_SHOPPING foreign key ("Time")
      references Shoppingcar ("Time")
      on update restrict
      on delete restrict;

alter table "Add"
   add constraint FK_ADD_ADD2_PRODUCT foreign key (Productid, Color, Size)
      references Product (Productid, Color, Size)
      on update restrict
      on delete restrict;

alter table Address
   add constraint FK_ADDRESS_UA_USER foreign key (Userid)
      references "User" (Userid)
      on update restrict
      on delete restrict;

alter table BS
   add constraint FK_BS_BS_BRAND foreign key (Brandid)
      references Brand (Brandid)
      on update restrict
      on delete restrict;

alter table BS
   add constraint FK_BS_BS2_STORE foreign key (Storeid)
      references Store (Storeid)
      on update restrict
      on delete restrict;

alter table Belong
   add constraint FK_BELONG_BELONG_STORE foreign key (Storeid)
      references Store (Storeid)
      on update restrict
      on delete restrict;

alter table Belong
   add constraint FK_BELONG_BELONG2_PRODUCT foreign key (Productid, Color, Size)
      references Product (Productid, Color, Size)
      on update restrict
      on delete restrict;

alter table Care
   add constraint FK_CARE_CARE_STORE foreign key (Storeid)
      references Store (Storeid)
      on update restrict
      on delete restrict;

alter table Care
   add constraint FK_CARE_CARE2_USER foreign key (Userid)
      references "User" (Userid)
      on update restrict
      on delete restrict;

alter table Landing
   add constraint FK_LANDING_QL_QQ foreign key (QQid)
      references QQ (QQid)
      on update restrict
      on delete restrict;

alter table Landing
   add constraint FK_LANDING_UL_USER foreign key (Userid)
      references "User" (Userid)
      on update restrict
      on delete restrict;

alter table Landing
   add constraint FK_LANDING_WL2_WECHAT foreign key (Weid)
      references WeChat (Weid)
      on update restrict
      on delete restrict;

alter table "Order"
   add constraint FK_ORDER_AO_ADDRESS foreign key (Consignee, Address)
      references Address (Consignee, Address)
      on update restrict
      on delete restrict;

alter table "Order"
   add constraint FK_ORDER_OU_USER foreign key (Userid)
      references "User" (Userid)
      on update restrict
      on delete restrict;

alter table PO
   add constraint FK_PO_PO_PRODUCT foreign key (Productid, Color, Size)
      references Product (Productid, Color, Size)
      on update restrict
      on delete restrict;

alter table PO
   add constraint FK_PO_PO2_ORDER foreign key (Orderid)
      references "Order" (Orderid)
      on update restrict
      on delete restrict;

alter table Purchase
   add constraint FK_PURCHASE_PURCHASE_PRODUCT foreign key (Productid, Color, Size)
      references Product (Productid, Color, Size)
      on update restrict
      on delete restrict;

alter table Purchase
   add constraint FK_PURCHASE_PURCHASE2_USER foreign key (Userid)
      references "User" (Userid)
      on update restrict
      on delete restrict;

alter table QQ
   add constraint FK_QQ_QL2_LANDING foreign key (QQid)
      references Landing (QQid)
      on update restrict
      on delete restrict;

alter table Shoppingcar
   add constraint FK_SHOPPING_VISIT2_USER foreign key (Userid)
      references "User" (Userid)
      on update restrict
      on delete restrict;

alter table "User"
   add constraint FK_USER_UL2_LANDING foreign key (Userid)
      references Landing (Userid)
      on update restrict
      on delete restrict;

alter table "User"
   add constraint FK_USER_VISIT_SHOPPING foreign key (Userid)
      references Shoppingcar (Userid)
      on update restrict
      on delete restrict;

alter table WeChat
   add constraint FK_WECHAT_WL_LANDING foreign key (Weid)
      references Landing (Weid)
      on update restrict
      on delete restrict;
