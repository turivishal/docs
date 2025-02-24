.. tip::

   This guide shows automatic {+dek-abbr-no-hover+} creation by using the
   ``createEncryptedCollection()`` function to create the {+qe+} collection.
   This call generates a ``keyId`` value for each encrypted field and returns
   those values in a new copy of the {+enc-fields-map+}.

   If you choose to provide an {+enc-fields-map+} in the automatic encryption
   options of a ``MongoClient`` that you use to read and write encrypted
   data, you need to specify the ``keyId`` values for each encrypted field.
   Therefore, you should save the {+enc-fields-map+} that
   ``createEncryptedCollection()`` returns for future use or assign
   ``keyAltNames`` for all the encrypted fields. This allows you to
   include the necessary ``keyId`` values in your client's
   {+enc-fields-map+}.

   To learn more about the contents of the encrypted fields map, see
   :ref:`qe-fundamentals-enable-qe`.

   To learn more about the ``createEncryptedCollection()`` function, see the
   API documentation (TODO: add appropriate link).
