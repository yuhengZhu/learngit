{\rtf1\ansi\ansicpg936\cocoartf1504
{\fonttbl\f0\fnil\fcharset0 Menlo-Regular;\f1\fnil\fcharset134 PingFangSC-Regular;}
{\colortbl;\red255\green255\blue255;\red0\green0\blue0;\red170\green13\blue145;\red28\green0\blue207;
\red196\green26\blue22;}
{\*\expandedcolortbl;\csgray\c100000;\csgenericrgb\c0\c0\c0;\csgenericrgb\c66500\c5200\c56900;\csgenericrgb\c11000\c0\c81000;
\csgenericrgb\c77000\c10200\c8600;}
\paperw11900\paperh16840\margl1440\margr1440\vieww10800\viewh8400\viewkind0
\deftab593
\pard\tx593\pardeftab593\pardirnatural\partightenfactor0

\f0\fs24 \cf2 \CocoaLigature0 [hud hide:\cf3 YES\cf2  afterDelay:\cf4 0\cf2 ];\
        \
        NSString *messageStr = [CommonMethod paramStringIsNull:message];\
        \
        UIAlertController *alertController = [UIAlertController alertControllerWithTitle:\cf3 nil\cf2  message:messageStr preferredStyle:UIAlertControllerStyleAlert];\
        \
        UIAlertAction *confirmAction = [UIAlertAction actionWithTitle:\cf5 @"
\f1 \'ce\'d2\'d6\'aa\'b5\'c0\'c1\'cb
\f0 "\cf2  style:UIAlertActionStyleDefault handler:\cf3 nil\cf2 ];\
        [alertController addAction:confirmAction];\
        \
        NSMutableAttributedString *alertMessageStr = [[NSMutableAttributedString alloc] initWithString:messageStr];\
        \
        [alertMessageStr addAttribute:NSFontAttributeName value:[UIFont systemFontOfSize:\cf4 9\cf2 ] range:NSRangeFromString(message)];\
        [alertMessageStr addAttribute:NSForegroundColorAttributeName value:COLOR_NORMAL_TEXT range:NSRangeFromString(message)];\
        [alertController setValue:alertMessageStr forKey:\cf5 @"attributedMessage"\cf2 ];\
        \
        [\cf3 self\cf2  presentViewController:alertController animated:\cf3 YES\cf2  completion:\cf3 nil\cf2 ];}