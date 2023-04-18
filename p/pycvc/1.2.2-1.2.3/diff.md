# Comparing `tmp/pycvc-1.2.2-py3-none-any.whl.zip` & `tmp/pycvc-1.2.3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,18 +1,18 @@
-Zip file size: 21984 bytes, number of entries: 16
+Zip file size: 22029 bytes, number of entries: 16
 -rw-r--r--  2.0 unx       34 b- defN 22-Aug-19 10:13 cvc/__init__.py
--rw-r--r--  2.0 unx      770 b- defN 23-Apr-17 12:22 cvc/_version.py
+-rw-r--r--  2.0 unx      770 b- defN 23-Apr-18 06:52 cvc/_version.py
 -rw-r--r--  2.0 unx     3507 b- defN 23-Mar-08 21:04 cvc/asn1.py
--rw-r--r--  2.0 unx     9235 b- defN 23-Apr-17 12:41 cvc/certificates.py
+-rw-r--r--  2.0 unx     9261 b- defN 23-Apr-18 06:46 cvc/certificates.py
 -rw-r--r--  2.0 unx    15209 b- defN 22-Aug-22 13:32 cvc/ec_curves.py
 -rw-r--r--  2.0 unx     8006 b- defN 22-Aug-23 11:50 cvc/oid.py
--rw-r--r--  2.0 unx     2484 b- defN 22-Aug-19 11:35 cvc/terminal.py
+-rw-r--r--  2.0 unx     2508 b- defN 23-Apr-18 06:51 cvc/terminal.py
 -rw-r--r--  2.0 unx     2639 b- defN 22-Aug-19 11:35 cvc/utils.py
 -rw-r--r--  2.0 unx        0 b- defN 22-Aug-17 12:41 cvc/tools/__init__.py
--rw-r--r--  2.0 unx    12792 b- defN 23-Apr-17 12:35 cvc/tools/cvc_create.py
+-rw-r--r--  2.0 unx    12838 b- defN 23-Apr-18 06:48 cvc/tools/cvc_create.py
 -rw-r--r--  2.0 unx     4829 b- defN 23-Apr-17 12:42 cvc/tools/cvc_print.py
--rw-r--r--  2.0 unx     5576 b- defN 23-Apr-17 13:34 pycvc-1.2.2.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Apr-17 13:34 pycvc-1.2.2.dist-info/WHEEL
--rw-r--r--  2.0 unx       92 b- defN 23-Apr-17 13:34 pycvc-1.2.2.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       14 b- defN 23-Apr-17 13:34 pycvc-1.2.2.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1185 b- defN 23-Apr-17 13:34 pycvc-1.2.2.dist-info/RECORD
-16 files, 66464 bytes uncompressed, 20072 bytes compressed:  69.8%
+-rw-r--r--  2.0 unx     5600 b- defN 23-Apr-18 06:54 pycvc-1.2.3.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Apr-18 06:54 pycvc-1.2.3.dist-info/WHEEL
+-rw-r--r--  2.0 unx       92 b- defN 23-Apr-18 06:54 pycvc-1.2.3.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       14 b- defN 23-Apr-18 06:54 pycvc-1.2.3.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1185 b- defN 23-Apr-18 06:54 pycvc-1.2.3.dist-info/RECORD
+16 files, 66584 bytes uncompressed, 20117 bytes compressed:  69.8%
```

## zipnote {}

```diff
@@ -27,23 +27,23 @@
 
 Filename: cvc/tools/cvc_create.py
 Comment: 
 
 Filename: cvc/tools/cvc_print.py
 Comment: 
 
-Filename: pycvc-1.2.2.dist-info/METADATA
+Filename: pycvc-1.2.3.dist-info/METADATA
 Comment: 
 
-Filename: pycvc-1.2.2.dist-info/WHEEL
+Filename: pycvc-1.2.3.dist-info/WHEEL
 Comment: 
 
-Filename: pycvc-1.2.2.dist-info/entry_points.txt
+Filename: pycvc-1.2.3.dist-info/entry_points.txt
 Comment: 
 
-Filename: pycvc-1.2.2.dist-info/top_level.txt
+Filename: pycvc-1.2.3.dist-info/top_level.txt
 Comment: 
 
-Filename: pycvc-1.2.2.dist-info/RECORD
+Filename: pycvc-1.2.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## cvc/_version.py

```diff
@@ -14,8 +14,8 @@
  * General Public License for more details.
  *
  * You should have received a copy of the GNU General Public License
  * along with this program. If not, see <http://www.gnu.org/licenses/>.
  */
 """
 
-__version__ = "1.2.2"
+__version__ = "1.2.3"
```

## cvc/certificates.py

```diff
@@ -77,15 +77,15 @@
         self.__a = self.__a.add_tag(0x5f29, to_bytes(val))
         return self
 
     def pubkey(self, pubkey=None, scheme=None, full=None):
         if (self.__data != None):
             return self.body().find(0x7f49)
         if (isinstance(pubkey, rsa.RSAPublicKey)):
-            pubctx = [pubkey.public_numbers().n, pubkey.public_numbers().e]
+            pubctx = {1: to_bytes(pubkey.public_numbers().n), 2: to_bytes(pubkey.public_numbers().e)}
         elif (isinstance(pubkey, ec.EllipticCurvePublicKey)):
             dom = ec_domain(pubkey.public_numbers().curve)
             Y = pubkey.public_bytes(Encoding.X962, PublicFormat.UncompressedPoint)
             if (full):
                 pubctx = {1: dom.P, 2: dom.A, 3: dom.B, 4: dom.G, 5: dom.O, 6: Y, 7: dom.F}
             else:
                 pubctx = {6: Y}
```

## cvc/terminal.py

```diff
@@ -32,15 +32,15 @@
 
     def to_bytes(self):
         x = 0
         total = len(self._args)
         for ix, attr in enumerate(self._args):
             x = x + 2**(total-ix-1) * getattr(self, attr, 0)
         x = x + self.role * 2**(total)
-        return to_bytes(x)
+        return x.to_bytes((total + 7) // 8, 'big')
 
 class TypeIS(Type):
     OID = oid.ID_IS
     name = 'TypeIS'
     _args = ('rfu5', 'rfu4', 'rfu3', 'rfu2', 'iris', 'finger')
     def __init__(self, role, **kwargs):
         for attr in self._args:
```

## cvc/tools/cvc_create.py

```diff
@@ -168,15 +168,15 @@
                 pub_key = serialization.load_pem_public_key(pubdata)
     elif (args.request):
         with open(args.request, 'rb') as f:
             data = f.read()
             puboid = CVC().decode(data).pubkey().oid()
             chr = CVC().decode(data).chr()
             if (scheme_rsa(puboid)):
-                pub_key = rsa.RSAPublicNumbers(CVC().decode(data).pubkey().find(0x82).data(), CVC().decode(data).pubkey().find(0x81).data()).public_key()
+                pub_key = rsa.RSAPublicNumbers(int.from_bytes(CVC().decode(data).pubkey().find(0x82).data(), 'big'), int.from_bytes(CVC().decode(data).pubkey().find(0x81).data(), 'big')).public_key()
             else:
                 curve = CVC().decode(data).find_domain()
                 Q = CVC().decode(data).pubkey().find(0x86).data()
                 pub_key = ec.EllipticCurvePublicKey.from_encoded_point(curve, bytes(Q))
     else:
         if (args.sign_as and args.type and not args.outer_as and not args.outer_key):
             if (isinstance(sign_key, rsa.RSAPrivateKey)):
```

## Comparing `pycvc-1.2.2.dist-info/METADATA` & `pycvc-1.2.3.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pycvc
-Version: 1.2.2
+Version: 1.2.3
 Summary: Card Verifiable Certificate tools
 Home-page: https://github.com/polhenarejos/pycvc
 Author: Pol Henarejos
 Author-email: pol.henarejos@cttc.es
 License: GPLv3
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Plugins
@@ -75,15 +75,15 @@
 cvc-create --role=dv_domestic --type=at --chr=ZZATDVCA00001 --valid=180 --sign-key=ZZATCVCA00001.pkcs8 --scheme=ECDSA_SHA_256 --sign-as=ZZATCVCA00001.cvcert --public-key=ZZATDVCA00001.pub
 ```
 
 3- Create a certificate request
 ```bash
 openssl ecparam -out ZZATTERM00001.pem -name prime256v1 -genkey
 openssl pkcs8 -topk8 -nocrypt -in ZZATTERM00001.pem -outform DER -out ZZATTERM00001.pkcs8
-cvc-create --chr=ZZATTERM00001 --scheme=ECDSA_SHA_256 --sign-key=ZZATTERM00001.pkcs8 --out-cert=ZZATTERM00001.cvreq
+cvc-create --chr=ZZATTERM00001 --scheme=ECDSA_SHA_256 --sign-key=ZZATTERM00001.pkcs8 --out-cert=ZZATTERM00001.cvreq --req-car=ZZATDVCA00001
 ```
 
 4- Sign a certificate request
 ```bash
 cvc-create --role=terminal --type=at --valid=60 --sign-key=ZZATDVCA00001.pkcs8 --sign-as=ZZATDVCA00001.cvcert --request=ZZATTERM00001.cvreq
 ```
```

